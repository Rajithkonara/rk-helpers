---
layout: default
---
#### Docker Basics
Running a container.

`search docker images `
```bash
$ docker serach <image name>
```
`Run a container `
```bash
$ docker run -d redis     ||    -d run in background
```
`Details about running container`
```bash
$ docker inspect <friendly-name|container-id>
```
`Logs`
```bash
$ docker logs <friendly-name|container-id>
```
`Tail Logs`
```bash
$ docker logs --follow <friendly-name|container-id>
```
`Accessing container`
```bash
$ docker run -d --name redisHostPort -p 6379:6379 redis:latest
```
`Run Multiple instances`
```bash
$ docker run -d --name redisDynamic -p 6379 redis:latest
```
`Check port`
```bash
$ docker port redisDynamic 6379
```
***`Persisting Data in the container`***

Containers are designed to be stateless. Bind volumes /dir is done by using -v option <host-dir>:<container-dir>

Redis image stores logs and data into a /data directory.

Any data which needs to be saved on the Docker Host, and not inside containers, should be stored in /opt/docker/data/redis.
```bash
$ docker run -d --name redisMapped -v /opt/docker/data/redis:/data redis
```
`Running a container in the foreground`
```bash
$ docker run -it ubuntu bash
```
