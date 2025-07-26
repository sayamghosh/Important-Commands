Here are the **basic Docker commands** in Markdown format:

````markdown
# 🐳 Basic Docker Commands

## 🔧 Installation Check
```bash
docker --version
````

## 🚀 Docker Container Lifecycle

### Run a container

```bash
docker run hello-world
```

### Run a container in interactive mode

```bash
docker run -it ubuntu
```

### Run a container in detached mode

```bash
docker run -d nginx
```

### List running containers

```bash
docker ps
```

### List all containers (including stopped)

```bash
docker ps -a
```

### Start a stopped container

```bash
docker start <container_id>
```

### Stop a running container

```bash
docker stop <container_id>
```

### Restart a container

```bash
docker restart <container_id>
```

### Remove a container

```bash
docker rm <container_id>
```

## 📦 Docker Images

### List all images

```bash
docker images
```

### Pull an image from Docker Hub

```bash
docker pull <image_name>
```

### Build an image from a Dockerfile

```bash
docker build -t <your_image_name> .
```

### Remove an image

```bash
docker rmi <image_name>
```

## 🛠️ Dockerfile

### Sample Dockerfile

```dockerfile
FROM node:18
WORKDIR /app
COPY . .
RUN npm install
CMD ["node", "index.js"]
```

## 📂 Volumes & Ports

### Run a container with port mapping

```bash
docker run -p 8080:80 nginx
```

### Run with volume binding

```bash
docker run -v $(pwd):/app myimage
```

## 🧹 Clean Up

### Remove all stopped containers

```bash
docker container prune
```

### Remove all unused images

```bash
docker image prune
```

## 🧪 Docker Compose (basic)

### Start services

```bash
docker-compose up
```

### Start in detached mode

```bash
docker-compose up -d
```

### Stop services

```bash
docker-compose down
```

---
```bash
docker exec -it <container_id_or_name> bash

```
