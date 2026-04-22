# 🎮 2048 Game Deployment on AWS EKS

## 📌 Project Overview
This project demonstrates how to deploy a containerized 2048 game on Kubernetes using AWS EKS.

## ⚙️ Tech Stack
- Docker
- Kubernetes
- AWS EKS
- NGINX

## 🚀 Deployment Steps

```bash
docker build -t suchit10/2048:v1 .
docker push suchit10/2048:v1

kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
