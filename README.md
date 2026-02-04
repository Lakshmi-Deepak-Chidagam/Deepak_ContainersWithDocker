1. Objective

The objective of this assignment is to install Docker Desktop and build a multi-container microservice application using Python Flask, Redis, and PostgreSQL. This hands-on helps in understanding containerization and Docker Compose.

2. Tools and Technologies Used

Docker Desktop

Docker Compose

Python Flask

Redis

PostgreSQL

GitHub

3. Implementation Steps
Step 1: Docker Installation

Docker Desktop was installed and verified using:

docker -v

Step 2: PostgreSQL Setup

PostgreSQL container was created using:

docker pull postgres
docker run -d -p 5432:5432 --name postgres1 -e POSTGRES_PASSWORD=pass12345 postgres

Step 3: Application Setup

The Flask application, Dockerfile, and compose.yaml were created.
Redis was configured using Docker Compose.

Step 4: Running the Application

The application was started using:

docker compose up 


The application was accessed using:

http://localhost:8000

4. Output

The following outputs were obtained:

Docker Desktop showing running containers
<img width="975" height="609" alt="image" src="https://github.com/user-attachments/assets/db4d3214-3f07-4c6a-96b2-5cb15ca46d1e" />

Web application output in browser

<img width="975" height="609" alt="image" src="https://github.com/user-attachments/assets/ef101e89-fe26-41a0-a649-2ec078ac5039" />

Issues Screenshot

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/164bdf08-3925-4c0b-a303-0b8dd56865c5" />

5. Errors Faced and Solutions
Error 1: Docker Pull 500 Error

Docker returned internal server error.

Solution:
Restarted Docker Desktop and WSL.

Error 2: Empty Compose File

Docker showed "empty compose file" error.

Solution:
Fixed build configuration in compose.yaml.

All errors were logged in GitHub Issues.

6. Learning Outcomes

From this assignment, I learned:

How Docker containers work

How to use Docker Compose

How containers communicate

How to debug Docker issues

How to document projects on GitHub

This hands-on improved my understanding of cloud-based application deployment.
