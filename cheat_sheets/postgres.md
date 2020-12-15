# Postgres

## Install and problems
### Env flag problem
```
export LDFLAGS="-L/usr/local/opt/openssl/lib"
or
env LDFLAGS="-I/usr/local/opt/openssl/include -L/usr/local/opt/openssl/lib" pip install psycopg2
```
### Wrong postgres versions
```
rm -rf /usr/local/var/postgres && initdb /usr/local/var/postgres -E utf8 - если неверные файлы для версии postgres
```
### List processes
```
ps -ef | grep postgres
```
### Psql error:
```
psql: error: could not connect to server: could not connect to server: No such file or directory
/usr/local/var/postgres/postmaster.pid
```

### Run postgres in docker
```
docker run -d --name postgres_12 -e POSTGRES_PASSWORD=postgres -p 127.0.0.1:5432:5432 -v $(pwd):/var/lib/postgresql/data postgres

docker exec -it postgres_12 psql -U postgres

psql -U postgres -h localhost
```

## Features
