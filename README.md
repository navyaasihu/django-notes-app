# Dockerized Django Notes App

This project is a **Dockerized version** of the original **django-notes-app**, forked from:  
https://github.com/LondheShubham153/django-notes-app

In this fork, **Docker-related changes have been added** to simplify setup, deployment, and environment consistency.

---

## 🚀 What Was Added in This Fork

The following files were added to enable Docker-based deployment:

- **Dockerfile** – Containerizes the Django backend application
- **docker-compose.yml** – Orchestrates Django, MySQL, and NGINX services
- **default.conf** – NGINX configuration file acting as a reverse proxy

These additions allow the entire application stack to run using Docker with minimal setup.

---

## 🏗️ Tech Stack

- **Frontend:** React (pre-built static files)
- **Backend:** Django
- **Reverse Proxy:** NGINX
- **Database:** MySQL
- **Containerization:** Docker & Docker Compose
- **Deployment:** AWS EC2 / Linux

---

## 📁 Project Architecture

Browser -> NGINX -> Django Application -> MySQL Database

## Installation
1. Clone the repository
```
git clone https://github.comnavyaasihu/django-notes-app.git
```

2. Build the app
```
docker build -t notes-app .
```

3. Run the app
```
docker run -d -p 8000:8000 notes-app:latest
```

## Nginx

Install Nginx reverse proxy to make this application available

`sudo apt-get update`
`sudo apt install nginx`


