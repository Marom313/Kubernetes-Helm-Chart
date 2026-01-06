# Helm Nginx Chart – Kubernetes

This repository contains a production-style Helm chart that deploys an Nginx application on Kubernetes.  
The project was built and tested on **Minikube (Windows)** and focuses on real-world DevOps practices, debugging, and Kubernetes networking behavior.

---

## 🚀 Project Goals

- Build a Helm chart from scratch (no auto-generated templates)
- Deploy an Nginx application using Kubernetes best practices
- Understand and debug Kubernetes Services and networking
- Work with Helm releases, dry-runs, and validation
- Handle Minikube-specific networking behavior on Windows

---

## 🧱 Architecture Overview

The Helm chart deploys the following Kubernetes resources:

- **Deployment**
  - Runs the Nginx container
  - Uses label-based selectors
- **Service (NodePort)**
  - Exposes the application internally and externally
- **Helm Chart**
  - Manages the full lifecycle as a single release

---

## 📂 Repository Structure

```text
myhelmchart/
├── Chart.yaml
├── values.yaml
├── templates/
│   ├── deployment.yaml
│   ├── service.yaml
│   └── NOTES.txt
└── charts/
