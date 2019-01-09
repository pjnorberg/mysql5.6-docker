# MySQL 5.6 in Docker
A simple way of running specific versions of MySQL in a
docker container with data persisted to `/data`. By default
it creates a `docker` user with password `docker` (so only suitable
for local development).

## Running service
To start the service (as detached), simply run up:
```
$ docker-compose up -d
```

## Stopping service
```
$ docker-compose down
```

## Stopping service and removing data
```
$ docker-compose down --volumes
```

## How to connect (Mac OS X)
```
SENSITIVE_DATABASE_CONNECTIONS_MYSQL_HOST=host.docker.internal
```