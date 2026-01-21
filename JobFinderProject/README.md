# JobFinder - DevOps & DevSecOps Portfolio Project (Jenkins CI/CD)

## Overview
**JobFinder** is a full-stack web application (Node.js + Express backend, React frontend) deployed using **modern DevOps and DevSecOps practices**.

This project demonstrates:

- **Containerization:** Docker images for backend & frontend
- **Orchestration:** Deployment to **K3s (lightweight Kubernetes)**
- **CI/CD:** Automated pipeline using **Jenkins**
- **DevSecOps:**
  - **SAST & SCA:** SonarQube scans
  - **Secret scanning:** Gitleaks
  - **DAST:** OWASP ZAP

> ⚠️ **Note:** This repository focuses on DevOps/DevSecOps practices. Minimal placeholder code is included; app logic itself is not the focus.

---

## Folder Structure

jobfinder/
├── docker/ # Dockerfiles & docker-compose
├── k3s-deployment.yaml # Kubernetes manifests
├── jenkins/ # Jenkins pipeline & scripts
├── devsecops/ # SonarQube, Gitleaks, DAST configs
└── README.md


---

## Docker Setup

**Dockerfiles** for backend & frontend allow containerized deployment.

**Build & Run locally using Docker Compose:**
```bash
cd docker
docker-compose up -d

Kubernetes Deployment (K3s)

Deploy services using K3s manifests
----------------------------------------------
## Jenkins CI/CD Pipeline

Pipeline location: jenkins/Jenkinsfile

Pipeline stages:

Checkout source code

Build Docker images for backend & frontend

Run SonarQube scan (SAST & SCA)

Run Gitleaks (secret scanning)

Run DAST with OWASP ZAP

Deploy to K3s cluster

Notify team (email)
