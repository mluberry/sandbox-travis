# Travis Sandbox project

[![Build Status](https://travis-ci.org/mluberry/sandbox-travis.svg?branch=master)](https://travis-ci.org/mluberry/sandbox-travis)

## Docker

### Install

```bash
brew install docker-machine docker docker-compose
docker-machine create --driver virtualbox dev
docker-machine start dev
docker-machine ls
docker-machine env dev
```

### Basic commands

#### Build containers
``docker-compose build``

#### Start containers
``docker-compose up -d``

#### Stop containers
``docker-compose stop``

#### Show containers logs
``docker-compose logs``

#### Remove containers
``docker-compose rm``

#### Remove containers and volumes
``docker-compose rm -v``

#### Shell (current container)
``docker exec -it sandboxtravis_app_1 bash``

#### Shell (create temporary container)
``docker-compose run --entrypoint bash --rm app``
