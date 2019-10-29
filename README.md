# learn-redis

* **redis-cli** open the redis
* **SET server:name "ikhda"** => to set the server name
* **GET server:name** => output will be "ikhda" because we has been declared the server name before
* **SET connections 10** => change SET to SETNX (SET-if-not-exists) if necessary
* **INCR connections** => incrementing the data we set before
* **DEL connections** => delete the data
* **SET resource:lock "Redis Demo"** => set the data
* **EXPIRE resource:lock 20** => set the data to be expired in 20 seconds
* **TTL resource:lock** => check the data, if expired will output -2 or -1 if the expiration not set, either will output the time left
* **RPUSH friends "Alice"** => will push data to array and in the right (tail)
* **LPUSH friends "Sam"** => will push data to array and in the left (head)
* **LRANGE friends 0 -1** => show the data between 0 index to the last, we can change 0 with the index we want and also for -1
* **LLEN friends** => return the length of the data
* **LPOP friends** => remove the first element (left)
* **RPOP friends** => remove the last element (right)