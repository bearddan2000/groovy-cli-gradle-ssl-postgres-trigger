# groovy-cli-gradle-ssl-postgres-trigger

## Description
Creates a small database table
called `dog` with an `insert update delete after` triggers.

All output normally
seen in a terminal will be in `groovy-srv/log` which will dump to the screen. The project may seem to hang but the logs from the container must be written to the project this can take up to 3 min.

Uses self-sign ssl.

## Tech stack
- groovy
- gradle
  - log4j
  - postgres driver

## Docker stack
- alpine:edge
- postgres:alpine
- gradle:jdk11

## To run
`sudo ./install.sh -u`
Creates groovy-srv/log

## To stop
`sudo ./install.sh -d`
Removes groovy-srv/log

## For help
`sudo ./install.sh -h`
