---
title: "Mastering Docker Commands"
seoTitle: "docker"
seoDescription: "essential docker commands"
datePublished: Sat Feb 01 2025 13:01:16 GMT+0000 (Coordinated Universal Time)
cuid: cm6m7bz3o000409jr1s0gene8
slug: mastering-docker-commands
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1738414695645/42afd759-fcc1-43e3-9e51-1ea0c9eecfe8.png
tags: docker, aws, development, developer, devops, docker-compose, aws-certified-solutions-architect-associate, devops-articles, docker-network

---

Docker has revolutionized the way we develop,ship and run applications by providing lightweight, portable and scalable containerization technology. Now a days understanding docker commands can greatly enhance your efficiency in managing containerized application.

This Guide helps in understanding the essential docker commands.

### Install docker through [docker official site](https://docs.docker.com/engine/install/)

### Check docker version

Ensure Docker is installed correctly by checking the version:

```plaintext
docker --version
```

### Get help with Docker Commands

If you're ever unsure about a Docker command, use:

```plaintext
docker help
```

## Managing Docker images and containers

### listing docker images

To list all available Docker images on your system

```plaintext
   docker images
```

### list running containers

To view active containers:

```plaintext
docker ps
```

### list all containers (running+stopped)

To display all containers, including stopped ones:

```plaintext
docker ps -a
```

### Run a container

To start a container using a specific image:

```plaintext
docker run hello-world
```

### Stop a container

To stop a running container:

```plaintext
docker stop <container-id>
```

### Start a container

To restart a stopped container:

```plaintext
docker start <container-id>
```

### Remove a container

To delete a stopped container:

```plaintext
docker rm <container-id>
```

#you can only remove a stopped a container.

### Inspect a container

To retrieve detailed information about a container:

```plaintext
docker inspect <container-id>
```

### Check logs of a container

To view logs from a container:

```plaintext
docker log <container-id>
```

### Rename a container

To rename an existing container:

```plaintext
docker rename <container-id> <new-name>
```

### Restart a container

To restart a running or stopped container:

```plaintext
docker restart <container-id>
```

### Run a container in background

To run a container in detached mode:

```plaintext
docker run -d <container-id>
```

### Run a container in foreground

To start a container and keep it attached to the terminal:

```plaintext
docker start -a <container-id>
```

### Start a shell inside a running container

To get interactive access to a container:

```plaintext
docker exec -it <container-id> /bin/bash
```

### Download an image from the docker registry

To pull an image from the Docker registry:

```plaintext
docker pull <image:tag>
```

### Delete an image

To remove an image from your system:

```plaintext
docker rmi <images>
```

### Build a docker image through Dockerfile

To create a new image using a Dockerfile:

```plaintext
docker build <image-name:tag> .
```

### Show stats of running containers

To monitor resource usage of containers:

```plaintext
docker stats
```

### Mapping ports

To map ports between the host and the container:

```plaintext
docker run -P <image_id>
```

### Kill a running container

To forcefully stop a container:

```plaintext
docker kill <container-id>
```

### Pause a running container

To temporarily suspend a container’s processes:

```plaintext
docker pause <container-id>
```

### Unpause a running container

To resume a paused container:

```plaintext
docker pause <container-id>
```

### Prune unused docker images

To delete unused images:

```plaintext
docker image prune
```

### Prune unused docker container

To delete stopped containers:

```plaintext
docker container prune
```

### History of a docker image

To check the history of an image:

```plaintext
docker history <image-id>
```

### Login to docker hub through CLI

To authenticate with Docker Hub:

```plaintext
docker login -u <username>
```

### Tag a docker image

To tag an image with a new repository and tag:

```plaintext
docker image tag old-username/old-image new-username/new-image:v1
```

### Push a image to docker registry

To push an image to Docker Hub:

```plaintext
docker push my-username/my-image
```

## **Conclusion**

Mastering Docker commands is essential for efficient container management and deployment. This guide has provided a structured approach to handling images, containers, and resources in Docker. With consistent practice, you'll be able to streamline your workflow and enhance your DevOps skills.

Happy Containerizing!