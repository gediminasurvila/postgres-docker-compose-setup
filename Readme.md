# PostgreSQL Docker Compose setup

## User Details

Username: `root`

Password: `password`

## Enter the Container w/ Bash

`docker-compose exec --user root db /bin/bash`

## Enter the Postgres Shell

`docker-compose exec --user root db psql -h localhost -U root`

## Create a DB

While inside the shell, run the following:

```
CREATE DATABASE "mydatabase";
```

## Conection string

`postgresql://root:password@localhost:5432/mydatabase`

## Drop DATABASE

`DROP DATABASE "mydatabase";`
