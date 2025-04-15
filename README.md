# Kubernetes Minikube Task - DevOps Internship

This repository contains the setup for a local Kubernetes cluster using Minikube, where a simple Node.js application is deployed and managed. The objective of this task was to understand and perform basic Kubernetes operations including deployments, services, scaling, and inspecting cluster resources.

## 🔧 Tools & Technologies Used

- Docker
- Kubernetes (via Minikube)
- kubectl
- Node.js
- Express.js

---

## 📁 Project Structure

k8s-minikube-task5/ │ ├── app/ # Node.js application │ ├── app.js │ ├── Dockerfile │ └── package.json │ ├── deployment.yaml # Kubernetes deployment ├── service.yaml # Kubernetes service (NodePort) └── screenshots/ # Screenshots of pod/service commands

---

## 🚀 Steps Performed

### 1. Minikube Setup
- Installed Minikube on Windows with Docker as the driver.
- Started the cluster using `minikube start`.

### 2. Application Setup
- Built a simple Express.js app that responds with "Hello from Kubernetes!".
- Created a Docker image and tagged it as `k8s-node-app`.

### 3. Kubernetes Deployment
- Created `deployment.yaml` to deploy the container with 1 replica.
- Created `service.yaml` to expose the deployment using NodePort.

### 4. Interacting with the Cluster
- Verified running pods and services using `kubectl get pods` and `kubectl get services`.
- Described pods for logs and debugging.
- Used `minikube service` command to access the app via browser.

### 5. Scaling the Deployment
- Scaled up the deployment to 3 replicas using:
- kubectl scale deployment node-app-deployment --replicas=3

- Verified multiple pods running.

---

## 📸 Screenshots

All relevant screenshots (pod listings, service output, scaling, browser output, etc.) are included in the `screenshots/` folder for reference.

---