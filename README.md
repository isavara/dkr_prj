This cheat sheet serves as a quick reference for developers, DevOps engineers, and sysadmins to work with Docker efficiently in a production environment.

---

## 🚀 Basic Commands

| Task | Command |
|------|---------|
| Check Docker version | `docker version` |
| View system-wide info | `docker info` |
| List all containers | `docker ps -a` |
| Start/Stop a container | `docker start <name>` / `docker stop <name>` |
| Remove a container | `docker rm <name>` |
| Remove an image | `docker rmi <image>` |

---

## 📦 Image Management

| Task | Command |
|------|---------|
| Build an image | `docker build -t <name>:<tag> .` |
| Pull an image | `docker pull <image>:<tag>` |
| Push an image | `docker push <image>:<tag>` |
| Tag an image | `docker tag <source> <target>` |
| List images | `docker images` |

---

## 🛠️ Container Lifecycle

| Task | Command |
|------|---------|
| Run a container | `docker run -d --name <name> <image>` |
| Execute in running container | `docker exec -it <name> /bin/bash` |
| View logs | `docker logs -f <name>` |
| Restart policy | `docker run --restart unless-stopped ...` |

---

## 🗃️ Volumes and Data Persistence

### Named Volume (Recommended for Production)

```bash
docker volume create db_data
docker run -v db_data:/var/lib/mysql ...
