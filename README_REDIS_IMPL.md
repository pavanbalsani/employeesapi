HOW TO START REDIS SERVER:
----------------------
1. In my laptop, redis is installed at C:\code\repos\redis>. 
   Open terminal in the installed path and execute **.\redis-server.exe** 
2. To run cli commands, execute .\redis-cli.exe from the installed path.
3. To shutdown redis, execute command **shutdown** from CLI and then execute **exit** command.

USEFUL COMMANDS:
---------------

1. To retrieve all keys in cache:
    127.0.0.1:6379> **keys ***
    "getAllEmployeesCache::SimpleKey []"
    "getEmployeeByIdCache::1"
2. Get details of a particular key:
   127.0.0.1:6379> **GET getEmployeeByIdCache::1**
   "\xac\xed\x00\x05sr\x00*com.example.demo.response.EmployeeResponsew\"\r\xc6\xf0\xfe\xf5\xb8\x02\x00\x04I\x00\x02idL\x00\x03aget\x00\x12Ljava/lang/String;L\x00\x05emailq\x00~\x00\x01L\x00\x04nameq\x00~\x00\x01xp\x00\x00\x00\x01t\x00\x0237t\x00\x17pavanbalasani@gmail.comt\x00\x05Pavan"
   1
3. flush/ remove all keys:
   127.0.0.1:6379> **FLUSHALL**
   OK

Resources Used for Redis Cache implementation:
----------------------------------------------
1. https://javatechonline.com/how-to-implement-redis-cache-in-spring-boot-application/
2. https://stackoverflow.com/questions/43111815/how-to-configure-redis-caching-in-spring-boot