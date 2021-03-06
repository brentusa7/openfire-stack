# Dockerized Openfire Server

This docker setup contains a stack with:
* openfire v4.2.3
* mysql v5.7
* adminer

## Requirements
* Docker
* Shell / Console (Git command line)


## Quickstart
Start Openfire using:

```bash
$ docker-compose up
```

## Services
* Openfire Admin Console > http://localhost:9090 
* phpMyAdmin > http://localhost:9000 
* MySQL Server > localhost:3306

## Openfire
Use this db settings in openfire initial setup:
* jdbc:mysql://database_srv:3306/openfire_db?rewriteBatchedStatements=true 
* user: openfire_db_user
* pwd: s3cr3t

## MySQL
Server exposes port 3306 to host with this credentials:
* user: root
* pwd: r00t

## Destroy Stack
```bash
$ docker-compose stop
$ docker-compose rm
$ docker system prune --force --volumes
```