# Docker
## Docker run
```
docker run -i -t <container name> /bin/bash        - запуск шела внутри контейнера. 

-it можно вместе
-d запуск в фоне

—link <container_name>:<host_name>

-h хост
--name - name
```

## Docker ps
```
docker ps - список контейнеров, docker ps -a - список всех, включая отсановленные
docker ps -aq -f status=exited - список остановленных контейнеров
```

## Docker logs
```
docker logs <container name> - список событий внутри контейнера
```

## Docker rm
```
docker rm <name> - удаление контейнера
```

## Docker commit
```
docker commit <name> <folder/imagename> - создание образа
```

## Docker build
```
docker build -t <path to image> <path to dockerfile>
```

## Docker pull
```
docker pull <name> - скачивание образа
```

## Run postgres in docker
```
docker run -d --name postgres_12 -e POSTGRES_PASSWORD=postgres -p 127.0.0.1:5432:5432 -v $(pwd):/var/lib/postgresql/data postgres

docker exec -it postgres_12 psql -U postgres

psql -U postgres -h localhost
```
