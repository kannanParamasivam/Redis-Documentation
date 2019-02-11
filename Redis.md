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
### Key Value oprations
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
* Set expiry when creating key value pair  
![Create key value with expiration][set_expiration_when_creating_key_value_pair]
* Persist expiring key value   
![Persist expiring key value][persist_expiring_key_value]
* Set multiple Key Values   
![Set multiple key values][mset]
* Append value of any key   
![Append value of any key][append]
* Rename any Key   
![Rename key][rename]
* **Scan** for keys
> * Scan in the cursor bases search where first time user passes cursor as 0 to start scan, the service returens next cursor value and result set, then the user have to pickup new cursor value and call scan command again. This will continue untill the cursor value returned by the service becomes 0 which mean full scan is completed.   
![Scan with cursor][scan]   
![Scan with pattern match][scan_w_patternmatch]
 ### List operations
 * Create list and show entire list   
 !["Create List"][create_list]
* Show part of the list
* Push value to the begining of the list   
![Push to the begining of the list][lpush]
### Set operations
> Sets are **unrodered** collection of **Unique strings**.
> * Read, Write and Remove takes **O(1) time**
> * Maximum **length** of set is **2^32 - 1** (i.e., 4 billion elements per set) 
* Create / Add item(s) to set   
![Create / Add item(s) to set][sadd]
* Check if a string **is member** of the set   
Is Member comparison is **case sensitive**   
![Check if a string is member of the set][sismember]
* **Show members** of the set   
![Show members of the set][smembers]
* **Scan** within a set with with and without pattern   
![Scan within a set with and withou pattern][sscan]
* **Show random member** from set   
![Show random member from set][srandmember]
* Show **number of members** in set   
![Shows number of members in set][scard]
* **Move** member from one set to another   
![Move member from one list to another][smove]
* **Remove** member(s) from set   
![Removemember(s) from set][srem]
* **POP random member** from set   
![POP random member from set][spop]
* **Difference** between the elements in first set and all the remaining sets   
![Difference between the first set and elements in remaining sets][sdiff]
* **Store the Difference** between elements in first set and elements in remaining sets   
![Store the Difference between elements in first set and elements in remaining sets][sdiffstore]
* **Intersection** between the sets and store results in another set   
![Intersection between the sets and store results in another set][sinterstore]




 [redis_install_command]: ./images/redis_install_command.JPG "Install redis"
 [open_redis_cli_command]: ./images/1_redis_open_cli.png "Open CLI"
 [ping_pong]: ./images/2_ping_pong.png "PING PONG"
 [quit_cli]: ./images/3_quit_redis_cli.png "Quit CLI"
 [set_get_key_value]: ./images/4_set_get_key_value.png "Set Get Key Value"
 [increment_decrement_value]: ./images/5_incr_decr.png "Increment / Decrement value"
 [exists_del_flushall]: ./images/6_exists_del_flushall.png "EXISTS DEL FLUSHALL"
 [key_space]: ./images/7_key_space.png "Create key within key space"
 [set_expiry_of_key_value]: ./images/8_expire.png "Set expiry of Key value"
 [set_expiration_when_creating_key_value_pair]: ./images/setex.JPG "Set expiry when creating key value pair"
 [persist_expiring_key_value]: ./images/persist.JPG "Persist expiring key value"
 [mset]: ./images/mset.JPG "Set multiple Key Values"
 [append]: ./images/append.JPG "Append value of any key"
 [rename]: ./images/rename.JPG "Rename key"
 [create_list]: ./images/create_list.JPG "Create List"
 [lpush]: ./images/lpush.JPG "Push to the begining of the list"
 [sadd]: ./images/sadd.JPG "Create / Add items to list"
 [sismember]: ./images/sismember.JPG "Check if a string is member of the set"
 [smembers]: ./images/smembers.JPG "Show members of the set"
 [scard]: ./images/scard.JPG "Shows number of members in set"
 [smove]: ./images/smove.JPG "Move member from one list to another"
[srem]: ./images/srem.JPG "Remove member(s) from set"
[sdiff]: ./images/sdiff.JPG "Difference between the first set and elements in remaining sets"
[sdiffstore]: ./images/sdiffstore.JPG "Store the Difference between elements in first set and elements in remaining sets"
[sinterstore]: ./images/sinterstore.JPG "Intersection between the sets and store results in another set"
[srandmember]: ./images/srandmember.JPG "Show random member from set"
[spop]: ./images/spop.JPG "POP random member from set"
[scan]: ./images/scan.JPG "scan for keys"
[scan_w_patternmatch]: ./images/scan_w_patternmatch.JPG "Scan with pattern match"
[sscan]: ./images/sscan.JPG "Scan within a set with and without pattern"