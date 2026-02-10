# Brain Tasks App – DevOps CI/CD Project

A full-stack task management application deployed using Docker, Kubernetes (EKS), and AWS CI/CD services.

---

## 🚀 Project Goal
Build and deploy a containerized web app using complete DevOps pipeline.

---

## 🧰 Tech Stack
- Docker
- Amazon ECR
- Amazon EKS (Kubernetes)
- AWS CodeBuild
- AWS CodePipeline
- GitHub
- kubectl / eksctl

---

## 🏗 Architecture Flow

GitHub → CodePipeline → CodeBuild → ECR → EKS → LoadBalancer → Users

---

## ⚙️ Setup Instructions

### Clone
git clone https://github.com/sooryas20-sudo/brain-tasks.git

### Build Docker image
docker build -t brain-app .

### Run locally
docker run -d -p 3000:80 brain-app

### Access
http://13.232.132.87:3000

---

## ☁️ CI/CD Pipeline

1. Code pushed to GitHub
2. CodePipeline triggers automatically
3. CodeBuild builds Docker image
4. Image pushed to Amazon ECR
5. Kubernetes pulls image and deploys to EKS
6. LoadBalancer exposes app

---

## 📦 Deployment

### Kubernetes
kubectl apply -f k8s/

### Check pods
kubectl get pods

### Check service
kubectl get svc

---

## ✅ Features Implemented
- Docker containerization
- ECR image registry
- EKS cluster deployment
- Automated builds using CodeBuild
- Automated CI/CD using CodePipeline
- Git version control
- LoadBalancer service

---

## 🌐 Live Application
http://aff1b68dd3d4a4f789b31b89aa46a722-1187586784.ap-south-1.elb.amazonaws.com/

---

## 📌 Author
Soorya S

