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


## 🌐 Architecture

User → NodePort → Kubernetes Service → Pod → Container

## 📸 Application Output
(<img width="1896" height="971" alt="Screenshot 2026-04-22 213431" src="https://github.com/user-attachments/assets/cba06d25-f15d-4cbd-9066-d8902ed4c8f7" />
)

## ⚠️ Challenges Faced

- Pods stuck in Pending (low resources)
- ImagePullBackOff (image not pushed)
- App not accessible (security group issue)
- Wrong context (Minikube vs EKS)

## 🙌 Credits

Base 2048 game from open-source project by Gabriele Cirulli  
This project focuses on deployment using DevOps practices
