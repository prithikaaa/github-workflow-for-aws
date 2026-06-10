# 🚀 Flask CI/CD Pipeline with GitHub Actions, Docker, AWS ECR & ECS

## 📌 Project Overview

This project demonstrates a complete **CI/CD pipeline** for a Flask web application using **GitHub Actions** and AWS services. It automates testing, Docker image creation, pushing to Amazon ECR, and deployment to Amazon ECS (Fargate/EC2).

The project showcases a real-world DevOps workflow from **code commit → automated build → containerization → cloud deployment**.

---

## 🏗️ Architecture

---

## ⚙️ Tech Stack

- Python (Flask)
- Docker
- Git & GitHub
- GitHub Actions (CI/CD)
- AWS EC2 (testing/optional)
- Amazon ECS (Fargate / EC2)
- Amazon ECR
- AWS IAM

---

## 🔄 CI/CD Pipeline Workflow

The pipeline runs automatically on every push to the `main` branch.

### CI (Continuous Integration)
- Checkout repository
- Setup Python environment (3.12)
- Install dependencies
- Compile Flask app for validation

### CD (Continuous Deployment)
- Configure AWS credentials (GitHub Secrets)
- Build Docker image
- Tag Docker image
- Push image to Amazon ECR
- Update ECS service for deployment

---

## 📁 Project Structure

---

## 🔐 GitHub Secrets Configuration

Add the following secrets in your GitHub repository:

- `AWS_ACCESS_KEY_ID`
- `AWS_SECRET_ACCESS_KEY`

These are used by GitHub Actions to authenticate with AWS securely.

---

## ☁️ AWS Services Used

### 1. Amazon EC2 (Optional)
- Used for manual testing of Flask app
- Access via public IP and port 5000

### 2. Amazon ECR
- Stores Docker images
- Acts as container registry for ECS

### 3. Amazon ECS (Fargate / EC2)
- Runs containerized Flask application
- Automatically updated via CI/CD pipeline

---

## 🚀 How Deployment Works

1. Developer pushes code to GitHub
2. GitHub Actions workflow is triggered
3. Docker image is built automatically
4. Image is pushed to Amazon ECR
5. ECS service pulls latest image
6. Updated application is deployed

---


### ECS Deployment (recommended)

---

## 📊 Features

- ✅ Automated CI/CD pipeline using GitHub Actions
- ✅ Docker containerization
- ✅ AWS ECR integration
- ✅ ECS deployment automation
- ✅ Secure credential management using GitHub Secrets
- ✅ End-to-end cloud deployment automation

---

## 🧠 Key Learnings

- CI/CD pipeline design using GitHub Actions
- Docker image creation and deployment
- AWS ECS and ECR integration
- IAM role and access key management
- Cloud-native deployment workflow
- Real-world DevOps automation

---

## 🔮 Future Improvements

- Add AWS Application Load Balancer (ALB)
- Use Terraform for Infrastructure as Code (IaC)
- Implement Blue-Green deployment strategy
- Add monitoring using AWS CloudWatch
- Add rollback strategy for ECS deployments

---

## 👩‍💻 Author

**Prithika Datta**  
B.Tech CSE | Cloud & DevOps Enthusiast

---

## ⭐ Project Summary

This project demonstrates a complete production-like CI/CD pipeline using GitHub Actions and AWS services, enabling fully automated deployment from code commit to cloud execution without manual intervention.
## 🌐 Application Access

### EC2 Deployment (if used)
