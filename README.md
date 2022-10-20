# Docker Tutorial
<p align='justify'>As name suggests this file is all about docker. In this file i will tell you about accessing docker images and containers. So without any further delay let's go.</p>

## Prerequisite
* Basic Knowledge on Docker.
* Basic linux commands.
* Docker setup in your pc

## Docker Commands 

* To pull the image from docker hub
```bash
    docker pull <image name/ID>
            
    docker pull python:latest
```
![docker pull](https://github.com/prasadmatta-github/docker_tutorial/blob/main/docker_images/docker_pull.png)

* To run the image.
```bash
    docker run <image name/ID>
            
    docker run python:latest
```
![docker run](./docker_images/docker_run.png)
> But the main difference between pull and run is, **pull** command will **download the image** from docker but **run** will **download the image** from docker hub **and create a container for it**.

* To check the images which is installed in your system
```bash
    docker images
```
![docker image](./docker_images/docker_images.png)

* To check the running containers 

```bash
    docker ps
```
![docker ps](./docker_images/docker_ps.png)

* To check all the containers
```bash
    docker ps -a
```
![docker ps a](./docker_images/docker_ps_a.png)

* To run the image
```bash
    docker run -d -p <local_port>:<container_port> <image_name/ID>
                            
    docker run -d -p 8000:80 python
```

* To run the image as a container in a detach mode and interactive mode 
```bash
    docker run -d -it --name <containername/ID> <imagename/ID> /bin/bash
                    
    docker run -d -it --name demo python /bin/bash  
```
![docker interactive](./docker_images/docker_inter.png)


* To start a container
```bash
    docker start <containername/ID>
            
    docker start demo
```
![docker start](./docker_images/docker_start.png)

* To enter into container 
```bash
    docker exec -it <container name/ID> /bin/bash
                
    docker exec -it demo /bin/bash
```
![docker execution](./docker_images/docker_exec.png)


# To learn more about docker
* [Docker Documentation](https://docs.docker.com/get-started/)









