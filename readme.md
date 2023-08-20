# Basic Docker Commands

This readme provides a quick reference for common Docker commands that are often used during development and managing Docker containers. These commands are a starting point for working with Docker images and containers.

## Docker Info

Get information about the Docker system:

```
docker info
```

## List Running Containers

List all running containers:

```
docker ps
```

List all containers, including stopped ones:

```
docker ps -a
```

## Building Images

Build a Docker image from a Dockerfile located in the current directory:

```
docker build .
```

Build an image and tag it with a specific name:

```
docker build -t <image-name> .
```

## Running Containers

Run a container using an image:

```
docker run <image-id>
```

Run a container and map ports:

```
docker run -p <host-port>:<container-port> <image-id>
```

## Stopping and Killing Containers

Stop a running container:

```
docker stop <container-id>
```

Kill a running container forcefully:

```
docker kill <container-id>
```

## Cleaning Up

Remove stopped containers, unused images, and networks:

```
docker system prune
```

Remove all cached build artifacts:

```
docker builder prune --all --force
```

## Running Commands Inside Containers

Run an interactive shell inside a running container:

```
docker exec -it <container-id> sh
```

## Running Specific Commands Inside Containers

Run a specific command inside a running container:

```
docker exec -it <container-id> <command>
```

## Summary

These basic Docker commands provide a foundation for interacting with Docker images and containers. They enable you to build, run, manage, and clean up containers effectively. As you become more familiar with Docker, you can explore more advanced commands and features to optimize your containerized development workflow.
