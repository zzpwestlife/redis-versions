# redis-versions

不同版本的 redis, 3/4/5/6/7 各一个

## 安装

```
git clone git@github.com:zzpwestlife/redis-versions.git
cd redis-versions
docker-compose up -d
```

## 使用

查看状态和端口

```
docker-compose ps
          Name                         Command               State            Ports
--------------------------------------------------------------------------------------------
docker-redis-old_redis3_1   docker-entrypoint.sh redis ...   Up      0.0.0.0:63793->6379/tcp
docker-redis-old_redis4_1   docker-entrypoint.sh redis ...   Up      0.0.0.0:63794->6379/tcp
docker-redis-old_redis5_1   docker-entrypoint.sh redis ...   Up      0.0.0.0:63795->6379/tcp
docker-redis-old_redis6_1   docker-entrypoint.sh redis ...   Up      0.0.0.0:63796->6379/tcp
docker-redis-old_redis7_1   docker-entrypoint.sh redis ...   Up      0.0.0.0:63797->6379/tcp
```

连接

```
docker-compose exec redis5 redis-cli
127.0.0.1:6379> ping
PONG
127.0.0.1:6379>
```

或者使用诸如 redis desktop manager 的 GUI 工具进行连接使用.
