# Redis #
>Service / In-Memory key value store. 
>* Stored in **cache memory**
>* Can store million records under 130 KB
>* Can do 110,000 SETs and 81,000 GETs per second
>* Can be converted as **persistent database**
>* Developed using **C**

## OS support
>Redis **officialy supports Linux, Unix and Mac**. For windows, Widows open source developers created a wrapper and made it working in windows

## Installation
* To install through web site, go to Redis website and download
* Following is the command to install using `apt-get` in Linux

    ![Install redis][redis_install_command]    

## Using Redis through CLI
* Open Redis CLI   
![Open CLI][open_redis_cli_command]
* Check if Redis is active   
![PING PONG][ping_pong]
* Quit CLI   
![Quit CLI][quit_cli]
* SET / GET Key Value   
![Set Get Key Value][set_get_key_value]
* Increment / Decrement value   
![Increment / Decrement value][increment_decrement_value]
* Check if a key exists, delete key value and delete all key values   
![EXISTS DEL FLUSHALL][exists_del_flushall]
* Create group of key values in Key Space   
![Create key within key space][key_space]
* Set expiry of key value in seconds   
![Set expiry of key value][set_expiry_of_key_value]
 



 [redis_install_command]: ./images/redis_install_command.JPG "Install redis"
 [open_redis_cli_command]: ./images/1_redis_open_cli.png "Open CLI"
 [ping_pong]: ./images/2_ping_pong.png "PING PONG"
 [quit_cli]: ./images/3_quit_redis_cli.png "Quit CLI"
 [set_get_key_value]: ./images/4_set_get_key_value.png "Set Get Key Value"
 [increment_decrement_value]: ./images/5_incr_decr.png "Increment / Decrement value"
 [exists_del_flushall]: ./images/6_exists_del_flushall.png "EXISTS DEL FLUSHALL"
 [key_space]: ./images/7_key_space.png "Create key within key space"
 [set_expiry_of_key_value]: ./images/8_expire.png "Set expiry of Key value"