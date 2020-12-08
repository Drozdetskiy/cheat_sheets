# TimescaleDB cheat sheet

## Docker run timescaledb
docker run -d --name timescaledb -p 127.0.0.1:5432:5432 -e POSTGRES_PASSWORD=postgres 
-v $(pwd):/var/lib/postgresql/data timescale/timescaledb:1.7.4-pg12


