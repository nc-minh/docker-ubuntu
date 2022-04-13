## Install on ubuntu with snap
```
sudo snap install docker 
```
## Check version
```
docker --version
```

## Check info
```
docker info
```

## See which containers are running
```
docker ps
```
## See which containers are running and containers stopped
```
docker ps -a
```

## Check what images are there
```
docker images
```

## Delete running and stopped containers (check with `docker ps -a`)
```
docker rm CONTAINER_ID
```

## Delete any images (can't be removed while the containers is running)
```
docker rmi REPOSITORY
```

## Run containers and show log in containers at cmd
```
docker run -it -p 8080:80 nginx
```
## Run containers and hide log in containers at cmd, just return containers id
```
docker run -d -p 8080:80 nginx
```

## Stop any running containers 
```
docker stop Containers_ID
```

## Set name of containers
```
docker run -d -p 8080:80 --name myName nameDefault
```
