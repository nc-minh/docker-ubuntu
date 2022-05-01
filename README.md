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
## Exit the command line but the container is still running
```
Ctrl + P, Ctrl + Q
```
## Run containers and hide log in containers at cmd, just return containers id
```
docker run -d -p 8080:80 nginx
```

## Stop any running containers 
```
docker stop Containers_ID
```
## Delete a running container
```
docker rm -f container_Name|container_ID
```

## Set name of containers
```
docker run -d -p 8080:80 --name myName nameDefault
```
## Access in containers is running
```
docker exec -it name bash
```
## Return to the terminal of the container
```
docker attach container_Name|container_ID
```

## Print out the log of running containers
```
docker logs containersName
```
## Build
```
docker build -t imageName pathOfDockFile(. is current folder)
```
## Docker-compose
```
docker-compose up -d
```
## Create a docker image from a container
```
docker commit container_Name|container_ID name:tag
```