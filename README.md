# 🚀 Flask Bootstrap Login & Dashboard Web App

![Python](https://img.shields.io/badge/Python-3.11-blue?style=for-the-badge&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-Web%20Framework-black?style=for-the-badge&logo=flask&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-5.3-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-Ready-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Render](https://img.shields.io/badge/Render-Deployed-46E3B7?style=for-the-badge&logo=render&logoColor=white)

A modern, responsive web application featuring a complete authentication system and a user dashboard. Built with **Flask**, **SQLite**, and **Bootstrap 5**, it includes secure session management, password hashing, native light/dark theme toggling, and is fully containerized for deployment.

---

## 🌐 Live Demo

The project is fully deployed on Render using Docker. You can test it live right now:

👉 **[Try the App on Render](https://python-flask-yluf.onrender.com)**

**How to test:**
1. Go to the *Create an account* page.
2. Create a new user with a password.
3. Log in with your new credentials to explore the secure Dashboard.

---

## 🐳 Docker Image (Docker Hub)

The Docker image repositories can be pulled directly from Docker Hub:

👉 **[avotraader/login-flask on Docker Hub](https://hub.docker.com/repository/docker/avotraader/login-flask/general)**

---

## 💻 Installation and Local Setup

Follow these exact steps to clone, configure, and execute this web interface locally on your machine.

### Prerequisites
Make sure you have **Python 3.x** installed on your system.

### 1. Set Up Your Project Folder
Navigate to your project directory inside your terminal:
```bash
# Clone the repository (if applicable) and navigate into it
# cd path/to/your/project

```

### 2. Configure Your Isolated Python Environment (venv)

It is highly recommended to use a virtual environment:

```bash
# Create the virtual environment
python -m venv .venv

# Activate the environment (Linux/macOS)
source .venv/bin/activate
# (On Windows, use: .\.venv\Scripts\activate)

```

### 3. Install Package Dependencies

```bash
pip install -r requirements.txt 

```

### 4. Run the App

```bash
python app.py

```

The application will be accessible at `http://localhost:5000`.

---

## 🐋 Docker Integration

If you prefer to run the application in an isolated container, follow these steps:

### 1. Build the Docker image

```bash
docker build -t mon-app-flask .

```

### 2. Run the Docker container

```bash
docker run -d -p 80:5000 --name flask-app-container mon-app-flask

```

*Open your browser and navigate to: [http://localhost:80*](http://localhost:80)

### 3. Stop the container

When you are finished, you can stop the running container with:

```bash
docker stop flask-app-container

```

---

## 📁 Project Structure

* `app.py`: Main backend logic, database initialization, and Flask routes.
* `users.db`: SQLite database (generated automatically upon first run).
* `Dockerfile`: Configuration for containerizing the application.
* `requirements.txt`: Python package dependencies.
* `templates/`: HTML views (`login.html`, `register.html`, `dashboard.html`) styled with Bootstrap 5.

```

```