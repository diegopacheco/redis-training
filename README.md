## Redis Training

#### Deck

https://www.slideshare.net/diego.pacheco/redis-218396098

#### Code 

###### Lettuce

https://github.com/diegopacheco/redis-training/tree/master/src/java-lettuce-redis-fun

```bash
./gradlew clean build
./gradlew run
```

###### Spring Data

https://github.com/diegopacheco/redis-training/tree/master/src/java-spring-data-redis-fun

```bash
./gradlew clean build
./gradlew run
```

### Running Redis 

#### Running the Server 

```bash
docker run redis
```
```
1:C 10 Jan 2020 17:36:01.963 # oO0OoO0OoO0Oo Redis is starting oO0OoO0OoO0Oo
1:C 10 Jan 2020 17:36:01.963 # Redis version=5.0.5, bits=64, commit=00000000, modified=0, pid=1, just started
1:C 10 Jan 2020 17:36:01.963 # Warning: no config file specified, using the default config. In order to specify a config file use redis-server /path/to/redis.conf
1:M 10 Jan 2020 17:36:01.966 * Running mode=standalone, port=6379.
1:M 10 Jan 2020 17:36:01.966 # WARNING: The TCP backlog setting of 511 cannot be enforced because /proc/sys/net/core/somaxconn is set to the lower value of 128.
1:M 10 Jan 2020 17:36:01.966 # Server initialized
1:M 10 Jan 2020 17:36:01.966 # WARNING overcommit_memory is set to 0! Background save may fail under low memory condition. To fix this issue add 'vm.overcommit_memory = 1' to /etc/sysctl.conf and then reboot or run the command 'sysctl vm.overcommit_memory=1' for this to take effect.
1:M 10 Jan 2020 17:36:01.966 # WARNING you have Transparent Huge Pages (THP) support enabled in your kernel. This will create latency and memory usage issues with Redis. To fix this issue run the command 'echo never > /sys/kernel/mm/transparent_hugepage/enabled' as root, and add it to your /etc/rc.local in order to retain the setting after a reboot. Redis must be restarted after THP is disabled.
1:M 10 Jan 2020 17:36:01.966 * Ready to accept connections
```

#### Running redis-cli

```bash
docker ps
docker exec -it $CONTAINER_ID(i.e b350a432b5af) redis-cli
```
```
127.0.0.1:6379> keys *
(empty list or set)
127.0.0.1:6379> 
```
