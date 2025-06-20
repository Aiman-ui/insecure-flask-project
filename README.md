#  Insecure Flask App - DevSecOps Mini Project

This intentionally vulnerable Flask application is designed for educational use in DevSecOps training. It contains poor security practices in both the application code and Dockerfile.

> **Purpose:** You will identify and fix basic security flaws, then run security scans using SonarQube (SAST) and Trivy (Docker image scanning).

---

## What's Wrong (By Design)

- Hardcoded credentials in the Flask app
- No input validation
- Debug route exposing system commands
- Weak session key
- Dockerfile uses unpinned base image
- Root user enabled in container
- No healthcheck, cleanup, or best practices

---

## 🧪 Tools to Use

You should use the following tools (already covered in class):

-  **SonarQube** – Static code analysis
-  **Trivy** – Docker image scanning
-  **Docker** – Build and run the app
-  **Git** – Clone and version changes

---

## 🧭 How to Run

```bash
# Step 1: Clone the Repo
git clone https://github.com/Aiman-ui/insecure-flask-project.git
cd insecure-flask-project

# Step 2: Build the Docker Image
docker build -t insecure-flask-app .

# Step 3: Run the App
docker run -p 5000:5000 insecure-flask-app

