
# 🐳 Docker Cheat Sheet

A comprehensive cheat sheet covering essential Docker commands, container lifecycle, image handling, volumes, networks, and more. Useful for beginners and advanced users alike.

---

## 🛠️ Docker Basics

### Check Docker Version
```bash
docker --version
docker version
```

### Get System Info
```bash
docker info
```

---

## 📦 Docker Images

### Pull an Image
```bash
docker pull <image_name>
```

### List Images
```bash
docker images
```

### Remove an Image
```bash
docker rmi <image_id>
```

---

## 🧱 Docker Containers

### Run a Container
```bash
docker run <image_name>
```

### Run with Custom Name
```bash
docker run --name my_container <image_name>
```

### Run in Detached Mode
```bash
docker run -d <image_name>
```

### Run with Interactive Terminal
```bash
docker run -it <image_name> /bin/bash
```

### Run and Remove After Exit
```bash
docker run --rm <image_name>
```

### List Running Containers
```bash
docker ps
```

### List All Containers
```bash
docker ps -a
```

### Stop a Container
```bash
docker stop <container_id_or_name>
```

### Start a Stopped Container
```bash
docker start <container_id_or_name>
```

### Remove a Container
```bash
docker rm <container_id_or_name>
```

---

## 🐳 Dockerfile & Image Build

### Build an Image
```bash
docker build -t my-image-name .
```

### Build with Dockerfile at Custom Path
```bash
docker build -f path/to/Dockerfile -t my-image-name .
```

---

## 🚀 Running Containers with Ports & Volumes

### Map Port
```bash
docker run -p 8080:80 <image_name>
```

### Mount Volume (Bind Mount)
```bash
docker run -v $(pwd):/app <image_name>
```

### Use Named Volume
```bash
docker volume create mydata
docker run -v mydata:/data <image_name>
```

---

## 🗃️ Docker Volumes

### Create a Volume
```bash
docker volume create myvolume
```

### List Volumes
```bash
docker volume ls
```

### Inspect a Volume
```bash
docker volume inspect myvolume
```

### Remove a Volume
```bash
docker volume rm myvolume
```

---

## 🌐 Docker Networks

### List Networks
```bash
docker network ls
```

### Create a Network
```bash
docker network create mynetwork
```

### Connect a Container to a Network
```bash
docker network connect mynetwork <container_name>
```

---

## 📊 Monitoring

### View Container Logs
```bash
docker logs <container_id_or_name>
```

### Stream Logs
```bash
docker logs -f <container_id_or_name>
```

### Resource Usage
```bash
docker stats
```

---

## 🧹 Clean Up

### Remove All Stopped Containers
```bash
docker container prune
```

### Remove All Unused Images
```bash
docker image prune
```

### Remove All Unused Volumes
```bash
docker volume prune
```

### Remove Everything (⚠️ Caution)
```bash
docker system prune -a
```

---

## 🏗️ Docker Compose

### Start Services
```bash
docker-compose up
```

### Start in Detached Mode
```bash
docker-compose up -d
```

### Stop Services
```bash
docker-compose down
```

### Build Images with Compose
```bash
docker-compose build
```

---

## 🧪 Advanced

### Execute a Command in Running Container
```bash
docker exec -it <container_name> <command>
```

### Copy File from Host to Container
```bash
docker cp local.txt <container_name>:/path/in/container/
```

### Copy File from Container to Host
```bash
docker cp <container_name>:/path/in/container/file.txt ./local.txt
```

---

## 📚 References

- [Docker Official Docs](https://docs.docker.com/)
- [Docker CLI Command Reference](https://docs.docker.com/engine/reference/commandline/cli/)

---

## 🙌 Contributing

Feel free to fork, star, and contribute with suggestions or pull requests.

---

Happy Dockering! 🐳
