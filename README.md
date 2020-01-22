# Simple Rest application using Spring boot, mongodb and docker

## Build the application

use maven to build and test the project.

```bash
mvn install
```

This will start the unit tests, package the application and then do the integration tests (before this docker-integration.yml will be started to have a mongodb instance) 

## Start the application on docker

```bash
docker-compose up -d
```

## Access to endpoints

```bash
http://localhost:8080/customers (to list all customers)
```