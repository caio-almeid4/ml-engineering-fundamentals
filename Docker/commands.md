
### Images

- **docker images**: lists all stored images
- **docker pull *image_name:version***: brings image to docker host
- **docker image inspect *image_name:version***: gets image information
- **docker build Dockerfile**: builds the image


### Containers

- **docker run *image_name:version**: creates a container from an image
	- **-d**: detach container from terminal
	- **-p host_port:container_port**: exposes container port to hosts network
- **docker ps**: lists running containers
	- **-a**: lists 
- **docker inspect *container_id**: gets container information
- **docker logs *container_id***: gets container logs
- **docker stop/kill/start/ *container_id*** : stops or starts a container
	- stop uses a SIGTERM message (process inside container have a time to shut down)
	- kill uses a SIGKILL message (process inside container shut down immediately)
	- docker forces kill if, after using stop, the container takes more than 10 seconds to stop
- **docker container stats *container_id***: monitors some container metrics (cpu, mem usage,...)
	- It's possible to use without *container_id*, in this case it wil show metrics from all running containers
- **docker exec *container_id***: executes commands inside the container
	- **-it *path***: allows to join on containers terminal and execute commands
* **docker rm *container_id***: removes a stopped container
* **docker container prune**: removes all stopped containers