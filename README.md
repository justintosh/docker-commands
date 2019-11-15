# docker and git commands
Frequently used docker commands

## Show all Containers

```
docker container ls -all
```

## Stop all Running Containers

```
docker stop $(docker ps -aq)
```

## Remove all Containers

```
docker rm $(docker ps -aq)
```

## Show all Images

```
docker images
```

## Remove all Images

```
docker rmi $(docker images -q)
```

## Force Remove Image

```
docker rmi -f <IMAGE ID>
```

## Run Command in An Already Running Container

```
docker exec -it [container-id] bash
```

## Latest MySQL image

```
docker pull mysql/mysql-server:latest
```

MySQL reference: https://dev.mysql.com/doc/mysql-installation-excerpt/5.5/en/docker-mysql-getting-started.html



------

Add submodule

```
git submodule add <REPO_URL>
```

Clone submodule

```
git submodule init
git submodule update
```

Pull update of submodules

```
git submodule update --init --recursive --remote
```




