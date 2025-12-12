
### Images

- **docker images**: lists all stored images
- **docker pull *image_name:version***: brings image to docker host
- **docker image inspect *image_name:version***: gets image information


### Containers

- **docker run *image_name:version**: creates a container from an image
	- **-d**: detach container from terminal
	- **-p host_port:container_port**: exposes container port to hosts network
- **docker ps: lists running containers
- **docker inspect *container_id**: gets container information
- **docker logs *container_id***: gets container logs
