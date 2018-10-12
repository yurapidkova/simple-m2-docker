# Simple docker compose config

## Workflow

### Base
```
docker-compose up -d
```
```
docker-compose down
```
```
docker ps
```


### php
If php docker file was changed
```
docker-compose build
```
### nginx
You can use `./docker/default.conf` config for small projects
Specific magento 2 config `./docker/nginx/m2.conf`

### Container 
`docker -it exec {container_name} /bin/bash -l`

### Logs 
`docker-compose logs -f` ||  `docker logs -f {container_name}`

### useful links

* [docker](https://docs.docker.com/install/)
* [docker-compose](https://docs.docker.com/compose/install/) 
