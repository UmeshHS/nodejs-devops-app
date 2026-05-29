# HerKey DevOps Intern Assignment

## Submitted By

**Name:** Umesh H S

## GitHub Repository

https://github.com/UmeshHS/nodejs-devops-app

## Docker Hub Repository

https://hub.docker.com/r/umesh12a/nodejs-devops-app


## Project Overview

This project demonstrates the deployment of a Node.js web application using modern DevOps practices including Docker, GitHub Actions CI/CD, Kubernetes deployment, and health monitoring.

---

## Technologies Used

* Node.js
* Express.js
* Docker
* Docker Hub
* GitHub Actions
* Kubernetes
* Minikube

---

## Features Implemented

* Docker containerization
* CI/CD pipeline automation
* Kubernetes deployment
* Health monitoring using liveness and readiness probes
* Automated Docker image build and push

---

## Application Endpoints

### Main Endpoint

```bash
/
```

### Health Endpoint

```bash
/health
```

---

## Docker Commands

### Build Docker Image

```bash
docker build -t nodejs-devops-app .
```

### Run Docker Container

```bash
docker run -p 3000:3000 nodejs-devops-app
```

---

## Kubernetes Deployment

### Deploy Application

```bash
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
```

### Verify Deployment

```bash
kubectl get pods
kubectl get svc
```

---

## CI/CD Workflow

GitHub Actions automatically:

1. Builds Docker image
2. Pushes image to Docker Hub
3. Triggers on every push to main branch

---

## Health Monitoring

Implemented using:

* Liveness Probe
* Readiness Probe

Endpoint used:

```bash
/health
```

---

## Troubleshooting

### Pod Failure

```bash
kubectl logs <pod-name>
```

### Deployment Details

```bash
kubectl describe deployment nodejs-devops-app
```

### Docker Issues

```bash
docker ps
docker images
```

---

## GitHub Repository

Repository contains:

* Application source code
* Docker configuration
* Kubernetes manifests
* GitHub Actions workflow

---

## Outcome

Successfully implemented an end-to-end DevOps deployment workflow using Docker, Kubernetes, and CI/CD automation.

## Cloud Compatibility

This project was demonstrated using Minikube for local Kubernetes deployment. The same Docker image and Kubernetes manifests can be deployed to cloud-managed Kubernetes services such as:

* AWS Elastic Kubernetes Service (EKS)
* Google Kubernetes Engine (GKE)

The deployment files are cloud-compatible and require minimal changes for production deployment.
