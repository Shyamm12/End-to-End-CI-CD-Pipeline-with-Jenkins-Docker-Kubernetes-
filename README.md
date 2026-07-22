# 🚀 End-to-End CI/CD Pipeline with Jenkins, Docker, Kubernetes & Argo CD

## 📌 Project Overview

This project demonstrates a complete DevOps CI/CD pipeline that automates the build, testing, containerization, and deployment of a Spring Boot application using modern DevOps tools and GitOps practices.

The application source code is hosted on GitHub. Jenkins continuously integrates the application, performs code quality analysis using SonarQube, builds a Docker image, pushes it to Docker Hub, and finally deploys the application to a Kubernetes cluster using Argo CD.

---

## 🎯 Objective

The objective of this project is to understand and implement an industry-standard CI/CD workflow by integrating:

- Git & GitHub
- Jenkins
- Maven
- SonarQube
- Docker
- Docker Hub
- Kubernetes (Minikube)
- Argo CD
- AWS EC2 (Jenkins Server)

---

## 🏗️ Project Architecture

```
        Developer
            │
            ▼
        GitHub Repository
            │
            ▼
      Jenkins (AWS EC2)
            │
            ├────────────► Maven Build
            │
            ├────────────► SonarQube Analysis
            │
            ├────────────► Docker Build
            │
            └────────────► Push Docker Image
                           │
                           ▼
                      Docker Hub
                           │
                           ▼
                    Kubernetes Cluster
                      (Minikube)
                           ▲
                           │
                      Argo CD (GitOps)
                           │
                           ▼
                Deploy Spring Boot Application
```

### Workflow

1. Developer pushes code to GitHub.
2. Jenkins automatically detects the changes.
3. Maven builds the Spring Boot application.
4. SonarQube performs static code quality analysis.
5. Jenkins builds a Docker image.
6. Docker image is pushed to Docker Hub.
7. Kubernetes deployment files stored in GitHub are monitored by Argo CD.
8. Argo CD automatically synchronizes the Kubernetes cluster with the latest manifests.
9. Spring Boot application is deployed successfully inside Kubernetes.

## 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| AWS EC2 | Hosted Jenkins Server |
| Git | Version Control |
| GitHub | Source Code Repository |
| Jenkins | Continuous Integration & Continuous Delivery |
| Maven | Build Automation Tool |
| SonarQube | Static Code Quality Analysis |
| Docker | Containerization |
| Docker Hub | Container Image Registry |
| Kubernetes (Minikube) | Container Orchestration |
| Argo CD | GitOps Continuous Deployment |
| Java 17 | Spring Boot Application Development |
| Spring Boot | Backend Application Framework |
| Linux (Ubuntu) | Server Environment |
| kubectl | Kubernetes Command Line Tool |
| eksctl | Kubernetes Cluster Management Tool |
