# 🚀 Django + Celery Project

A Dockerized Django application integrated with Celery for asynchronous task processing.

This project demonstrates:

- Running Django inside Docker
- Integrating Celery with Django
- Managing services using Docker Compose
- Handling proper Linux-compatible line endings
- Clean project structure for production-style setup

---

## 🛠 Tech Stack

- Python 3.11
- Django
- Celery
- Docker
- Docker Compose
- Alpine Linux (Docker base image)

---

## 📂 Project Structure

django_celery_project/
│
├── dcelery/
│   ├── dcelery/          # Django project settings
│   ├── Dockerfile
│   ├── entrypoint.sh
│   ├── manage.py
│   ├── requirements.txt
│   └── docker-compose.yml
│
├── .gitignore
├── .gitattributes
└── README.md

---

## ⚙️ Setup Instructions

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/aranya-code/django_celery_project.git
cd django_celery_project/dcelery

### 2️⃣ Build and Run the Project
docker compose up --build

### 🐳 Docker Configuration
Dockerfile

Uses python:3.11-alpine

Sets working directory

Installs dependencies from requirements.txt

Copies project files

Runs Django server

### 🐳 docker-compose.yml

Defines Django service

Exposes port 8001

Loads environment variables from .env



