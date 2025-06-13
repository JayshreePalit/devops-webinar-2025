# 📦 Day 4 – Docker Basics

## 📌 Objective:
Understand Docker fundamentals and perform hands-on tasks like installing Docker, running containers, and managing images.

---

## 🧠 What is Docker?

Docker is a platform that allows you to develop, ship, and run applications in lightweight, portable containers. It helps avoid the "it works on my machine" problem by standardizing environments.

---

## ✅ Key Docker Concepts:

| Term        | Description |
|-------------|-------------|
| **Image**   | Blueprint for a container (like an OS + app pre-installed). |
| **Container** | Running instance of an image. Lightweight and fast. |
| **Dockerfile** | Script to build Docker images automatically. |
| **Docker Hub** | Public registry to share/pull images. |

---

## 🔧 What I Did:

1. Installed Docker on Ubuntu using `apt`.
2. Verified installation with `docker --version`.
3. Ran the `hello-world` container.
4. Pulled and ran an NGINX container (`docker run -d -p 8080:80 nginx`).
5. Used commands like `docker ps`, `docker images`, and `docker stop`.
6. Removed unused containers/images with `docker system prune`.

---

## 📸 Screenshots:
![day4 1](https://github.com/user-attachments/assets/da8b8ac3-2d11-4127-b0ba-ef661bb130ef)
![day 4 2](https://github.com/user-attachments/assets/ff1d6660-fffe-4f33-af2c-9308030719a5)
![day 4 3](https://github.com/user-attachments/assets/c39118e8-1011-4870-8002-65be5c4a56a5)
![day4 4](https://github.com/user-attachments/assets/a96e58f9-9288-420b-a815-55645f39f7ea)
![day4 5](https://github.com/user-attachments/assets/f33fa58d-d2fa-4193-b3ed-ebdb07109fd4)
![day 4 image name changes](https://github.com/user-attachments/assets/e7cf7d51-a438-4c96-8e96-4f1b3d940ae3)
![day 4 push](https://github.com/user-attachments/assets/38bbf23a-4cdb-4770-995e-e33eb807b167)
![day4 docker](https://github.com/user-attachments/assets/ce7c9c3f-1930-48fc-ade8-d90802747c25)
![day4 complete](https://github.com/user-attachments/assets/8f21a8d8-fc6b-4111-aee7-329a163ab0e7)



> 💡 *All screenshots are stored in the `screenshots/` folder.*

---

## 🧠 Learnings:

- Docker is extremely fast and lightweight for testing apps.
- `docker run` is powerful and can be used with many flags (`-d`, `-p`, `--name`).
- Cleaning up resources is important to save space.
- The containerized NGINX was accessible via browser → `localhost:8080`.

---

## 📘 Commands Used:

```bash
sudo apt update
sudo apt install docker.io
docker --version
sudo systemctl start docker
sudo docker run hello-world
sudo docker run -d -p 8080:80 nginx
sudo docker ps
sudo docker images
sudo docker system prune
