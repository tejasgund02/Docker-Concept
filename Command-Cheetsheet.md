# 🐳 Docker Command Cheat Sheet

## 📌 Basic Commands
- Check Docker version:
  ```sh
  docker --version
  ```
- Show system-wide information:
  ```sh
  docker info
  ```
- List all available commands:
  ```sh
  docker --help
  ```

## 🚀 Container Management
- Run a container:
  ```sh
  docker run -d --name my_container nginx
  ```
- List running containers:
  ```sh
  docker ps
  ```
- List all containers (including stopped ones):
  ```sh
  docker ps -a
  ```
- Stop a container:
  ```sh
  docker stop my_container
  ```
- Start a stopped container:
  ```sh
  docker start my_container
  ```
- Remove a container:
  ```sh
  docker rm my_container
  ```

## 📦 Image Management
- List images:
  ```sh
  docker images
  ```
- Pull an image from Docker Hub:
  ```sh
  docker pull ubuntu
  ```
- Remove an image:
  ```sh
  docker rmi nginx
  ```

## 🛠️ Build and Push Images
- Build an image from a Dockerfile:
  ```sh
  docker build -t my_image .
  ```
- Tag an image:
  ```sh
  docker tag my_image myrepo/my_image:v1
  ```
- Push an image to Docker Hub:
  ```sh
  docker push myrepo/my_image:v1
  ```

## 🔗 Networking
- List networks:
  ```sh
  docker network ls
  ```
- Create a network:
  ```sh
  docker network create my_network
  ```
- Connect a container to a network:
  ```sh
  docker network connect my_network my_container
  ```
- Disconnect a container from a network:
  ```sh
  docker network disconnect my_network my_container
  ```

## 💾 Volume Management
- List volumes:
  ```sh
  docker volume ls
  ```
- Create a volume:
  ```sh
  docker volume create my_volume
  ```
- Remove a volume:
  ```sh
  docker volume rm my_volume
  ```
- Mount a volume to a container:
  ```sh
  docker run -d -v my_volume:/data --name my_container nginx
  ```

## 🏗️ Docker Compose
- Start services defined in `docker-compose.yml`:
  ```sh
  docker-compose up -d
  ```
- Stop services:
  ```sh
  docker-compose down
  ```
- Restart services:
  ```sh
  docker-compose restart
  ```
- Show logs:
  ```sh
  docker-compose logs
  ```

## 🧹 Cleanup
- Remove all stopped containers:
  ```sh
  docker container prune
  ```
- Remove all unused images:
  ```sh
  docker image prune
  ```
- Remove all unused volumes:
  ```sh
  docker volume prune
  ```
- Remove everything (containers, images, networks, and volumes):
  ```sh
  docker system prune -a
  ```

---
🚀 **Happy Dockering!**

