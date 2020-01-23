# Simple Rest application using Spring boot, mongodb and docker

## Build the application

use maven to build and test the project.

```bash
mvn clean install
```

This will start the unit tests, package the application and then do the integration tests (before this docker-compose.yml will be started for mongo-data-base service to have a mongodb instance) 

## Start the application on docker

```bash
docker-compose up -d
```
This will build a docker image using the Dockerfile, then start two containers the first is for the mongodb instance and the second for the customer app and link the two containers.

## Access to endpoints

```bash
http://localhost:8080/customers (to list all customers)
```