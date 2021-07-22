# Devops instructions

## Docker

Pieces of information about docker daemon
```
docker system info
```
Resource allocation (Docker resources usage)
```
docker system df
```
Docker images listing
```
docker images
```
Docker containers listing (active containers)
```
docker ps
```
Docker containers listing (all containers)
```
docker ps -a
```
Docker containers listing
```
docker volume ls
```
Docker volume metadata
```
docker volume inspect VOLUME_NAME
```
Manually remove (delete) Docker volume
```
docker volume rm VOLUME_NAME
```
Automatically remove (delete) Docker volume
```
docker volume prune
```
Run Docker containers
```
docker run -it --name ubuntu-1 ubuntu:18.04 bash
```
