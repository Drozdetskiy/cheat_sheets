# ClickHouse

## Install with docker
```
docker run -d --name clickhouse --ulimit nofile=262144:262144 --volume=$(pwd):/var/lib/clickhouse yandex/clickhouse-server 
```

## Connect from a native client
```
docker run -it --rm --link clickhouse:clickhouse-server yandex/clickhouse-client --host clickhouse-server
```

