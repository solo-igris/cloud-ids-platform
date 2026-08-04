# Docker Introduction

## What is Docker?

Docker is an **open-source platform** that allows developers to package an application along with all its dependencies into a **container**.

A container ensures that the application runs the same way on any computer, whether it is a developer's laptop, a testing server, or the cloud.

> **Build once, run anywhere.**

---

# Why Docker?

Without Docker, an application may work on one computer but fail on another because of differences in:

- Operating system
- Software versions
- Installed libraries
- Environment settings

Docker solves this problem by packaging everything the application needs into a single container.

---

# Where is Docker Used?

Docker is widely used in modern software development.

### Software Development
- Creates the same environment for developers and testers.

### Cloud Computing
- Deploy applications on AWS, Azure, and Google Cloud.

### Microservices
- Run each service in its own container.

### CI/CD
- Automate application testing and deployment.

### Machine Learning
- Create isolated environments for ML projects.

### IoT & Edge Computing
- Run lightweight applications on small devices.

---

# Advantages of Docker

- **Portability** – Run applications on any system with Docker installed.
- **Lightweight** – Uses fewer resources than virtual machines.
- **Scalable** – Easily run multiple containers.
- **Consistent** – Same environment for development, testing, and production.
- **Fast** – Containers start in seconds.

---

# Docker vs Traditional Deployment

| Feature | Traditional Deployment | Docker |
|---------|------------------------|--------|
| Environment | Different on each system | Same everywhere |
| Setup | Manual installation | Quick and automated |
| Dependencies | Can conflict | Packaged inside the container |
| Resource Usage | High | Low |
| Scalability | Difficult | Easy |

---

# Docker Components

## Docker Engine

The main service that builds, runs, and manages Docker containers.

---

## Docker Image

A **Docker Image** is a template that contains:

- Application code
- Libraries
- Dependencies
- Configuration

Images are used to create containers.

---

## Docker Container

A **Container** is a running instance of a Docker image.

It is isolated from the host system but shares the operating system kernel.

---

## Docker Hub

Docker Hub is an online repository where developers can:

- Download Docker images
- Share their own images

Example images:

- Ubuntu
- Nginx
- MySQL
- Redis

---

# How Docker Works

```text
Write Application
       ↓
Create Dockerfile
       ↓
Build Docker Image
       ↓
Run Docker Container
       ↓
Deploy Anywhere
```

---

# Benefits of Docker

- Eliminates the **"Works on my machine"** problem.
- Makes application deployment faster.
- Simplifies dependency management.
- Supports cloud deployment.
- Makes scaling applications easier.

---

# Summary

- Docker is a **containerization platform**.
- It packages applications and their dependencies into **containers**.
- Containers run consistently across different environments.
- Docker improves **portability**, **speed**, **scalability**, and **consistency**.
- The main Docker components are:
  - Docker Engine
  - Docker Images
  - Docker Containers
  - Docker Hub
