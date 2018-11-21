# docker-commands
Frequently used docker commands

## Stop all Running Containers

```
docker stop $(docker ps -aq)
```

## Remove all Containers

```
docker rm $(docker ps -aq)
```

## Remove all Images

```
docker rmi $(docker images -q)
```




## Latest MySQL image

```
docker pull mysql/mysql-server:latest
```

MySQL reference: https://dev.mysql.com/doc/mysql-installation-excerpt/5.5/en/docker-mysql-getting-started.html
