docker-oracle-xe-11g
============================

Oracle Express Edition 11g Release 2 on Ubuntu 14.04.1 LTS

This **Dockerfile** is a [trusted build](https://registry.hub.docker.com/u/wnameless/oracle-xe-11g/) of [Docker Registry](https://registry.hub.docker.com/).

### Installation
```
docker pull marcelmaatkamp/docker-oracle-xe-11g
```

Run with 22 and 1521 ports opened:
```
ddocker run -d --name oracle -p 49160:22 -p 49161:1521 marcelmaatkamp/docker-oracle-xe-11g
```

Connect database with following setting:
```
hostname: localhost
port: 49161
sid: XE
username: system
password: oracle
```

Password for SYS & SYSTEM
```
oracle
```

Login by SSH
```
ssh root@localhost -p 49160
password: admin
```
