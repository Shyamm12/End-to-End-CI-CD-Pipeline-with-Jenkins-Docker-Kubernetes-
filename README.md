# 🚀 End-to-End CI/CD Pipeline with Jenkins, Docker, Kubernetes & Argo CD

## 📌 Project Overview

This project demonstrates an end-to-end CI/CD pipeline for deploying a Spring Boot application using modern DevOps tools and practices.

The pipeline automates the complete software delivery process, starting from source code management to continuous deployment on a Kubernetes cluster using Argo CD.

## 🛠️ Tech Stack

- Java
- Spring Boot
- Maven
- Git & GitHub
- Jenkins
- SonarQube
- Docker
- Docker Hub
- Kubernetes (Minikube)
- Argo CD

---

# 🏗️ Project Architecture

```
Developer
    │
    ▼
GitHub Repository
    │
    ▼
Jenkins Pipeline
    │
    ├── Checkout Source Code
    ├── Build using Maven
    ├── SonarQube Code Analysis
    ├── Docker Image Build
    ├── Push Docker Image to Docker Hub
    └── Update Kubernetes Manifest
                    │
                    ▼
              GitHub Repository
                    │
                    ▼
                 Argo CD
                    │
                    ▼
             Kubernetes Cluster
                    │
                    ▼
        Spring Boot Application
```

---
