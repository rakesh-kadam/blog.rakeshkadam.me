## Useful Docker Command

Docker is used to build, share and deploy containerized applications. 


In this post, I’ll share essential docker commands that will help you steer through the world of Docker. 

Refer to this [link](https://docs.docker.com/engine/reference/commandline) for official documentation if you require additional optional along with below mentioned docker commands

**Docker Commands**
	
 List all running container 
```
$ docker ps 
```

List all running and stopped container
```
$ docker ps -a 
```

List all available docker images
```
$ docker images 
```

Download Image and/or Create a container 
```
$ docker run <image-name>:<image-tag> 
```

Download a docker image
```
$ docker pull <image-name>:<image-tag>
```
	
Append a command
```
$ docker run <image> bash
```

Execute a command
```
$ docker exec <contianer> cat /etc/hosts 
```

Detached mode (Runs in the background)
```
$ docker run -d <image-name> 
```

Attached mode
```
$ docker attach <contianer-id> 
```

Stop a container container
```
$ docker stop <container-id/name> 
```

Remove a docker container 
```
$ docker rm <contianer-id/name> 
```

Delete a docker image
```
$ docker rmi <image-id/name> 
```

Remove all unused containers, networks, images (both dangling and unreferenced), and optionally, volumes
```
$ docker system prune
```

Run interactive mode with terminal access 
```
$ docker run -it <image-name> 
```

Port mapping of docker host with container 
```
$ docker run -p <docker_host_port_number>:<container_port_number> <image-name> 
```

Volume mapping of docker host with container
```
$ docker run -v <docker_host_file_path>:<container_file_path> <image-name> 
```

Inspect docker container
```
$ docker inspect <contianer-id/name>
```

Check container logs
```
$ docker logs <contianer-id/name> 
```

**Note: **
- If you run a plain ubuntu image without any application in it the container will immediately exit as there would be no running process in it.
- You cannot add port mapping when the container is running

 