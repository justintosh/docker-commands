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

## Clear Docker Caches

```
docker system prune -a
```

## Run Command in An Already Running Container

```
docker exec -it [container-id] bash
```

## Docker-compose Up with Rebuild

```
docker-compose up --build
```

## Latest MySQL image

```
docker pull mysql/mysql-server:latest
```

MySQL reference: https://dev.mysql.com/doc/mysql-installation-excerpt/5.5/en/docker-mysql-getting-started.html



------

Add submodule

```
git submodule add <REPO_URL> [FOLDER_NAME]
```

Clone submodule

```
git submodule update --init --recursive
```

Pull update of submodules

```
git submodule update --recursive --remote
```

Update last commit message

```
git commit --amend
# make changes
Esc + :x + Enter on Vim to save and quit
git push --force
```

Merging multiple commits into one

```
git rebase -i HEAD~x
# make changes
Esc + :x + Enter on Vim to save and quit
# update commit messages, add # to ignore the line if necessary
Esc + :x + Enter on Vim to save and quit
git push origin <branch> -f
```

Reset the local branch to follow remote

```
git fetch origin
git reset --hard origin/master
```
