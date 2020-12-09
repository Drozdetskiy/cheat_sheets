# TimescaleDB cheat sheet

## Flag on install
```
ln -s /usr/local/Cellar/postgresql@12/12.5/include/postgresql/server /usr/local/Cellar/postgresql@12/12.5/include/server
```

## Docker run timescaledb
```
docker run -d --name timescaledb -p 127.0.0.1:5432:5432 -e POSTGRES_PASSWORD=postgres 
-v $(pwd):/var/lib/postgresql/data timescale/timescaledb:1.7.4-pg12
```

## Extend the database with TimescaleDB
```SQL
CREATE EXTENSION IF NOT EXISTS timescaledb;
```

