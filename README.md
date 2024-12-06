![Docker Logo]([https://upload.wikimedia.org/wikipedia/commons/3/39/Docker_logo.png](https://www.google.com/url?sa=i&url=https%3A%2F%2Fen.m.wikipedia.org%2Fwiki%2FFile%3ADocker_%2528container_engine%2529_logo.png&psig=AOvVaw2gYMaAR9i1CkiuYlR8R0Ui&ust=1733554711234000&source=images&cd=vfe&opi=89978449&ved=0CBQQjRxqFwoTCICDvtjIkooDFQAAAAAdAAAAABAJ))

# Docker Basics

This guide covers the fundamentals of Docker, including creating Docker images, building, running containers, and common Docker commands.

---

## What is Docker?

Docker is a platform for developing, shipping, and running applications in lightweight, portable containers. Containers are isolated environments that include everything needed to run an application, such as code, dependencies, and configurations.

---

## Key Concepts

- **Image**: A blueprint for a container, created using a Dockerfile.
- **Container**: A runtime instance of an image.
- **Dockerfile**: A script with instructions to create a Docker image.
- **Docker Hub**: A public repository to share and store Docker images.

---

## Basic Workflow

### 1. Install Docker

Download and install Docker from the [Docker website](https://www.docker.com/get-started).

### 2. Write a Dockerfile

A Dockerfile contains instructions for building an image. Here’s an example:

Create a file named `Dockerfile` in your project directory with the following content:

```dockerfile
# Use a lightweight base image
FROM alpine:latest

# Command to execute when the container starts
CMD ["echo", "Hello, World!"]
```
### 3. Steps to Build and Run this Dockerfile

Create a new directory and create a Dockerfile inside it.
Build the Docker image:

```bash
docker build -t hello-world-image .
```
Run the Docker container

```bash
docker run hello-world-image

```


