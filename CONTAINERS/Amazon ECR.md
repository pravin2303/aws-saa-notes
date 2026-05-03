# 🧠 Amazon ECR (Elastic Container Registry)

## 🔗 Service Type
#Containers #Registry #Docker #DevOps

---

## 📌 What is Amazon ECR?

Amazon ECR is a **fully managed container image registry** that allows you to:

- Store Docker images
- Manage container images securely
- Integrate with AWS container services

👉 ECR = “Docker Hub for AWS”

---

## ⚙️ How It Works (Architecture Thinking)

1. Build Docker image
2. Push image to ECR repository
3. Deploy using:
   - [[Amazon ECS]]
   - [[Amazon EKS]]
   - [[AWS Fargate]]

👉 Central storage for container images

---

## 🏗️ Core Components

### 1. Repository
- Stores container images

---

### 2. Image
- Docker image with app + dependencies

---

### 3. Image Tags
- Versioning (e.g., v1, latest)

---

## 🧠 Architectural Logic (Why ECR?)

### When to Choose ECR:

✅ Using containers (Docker)  
✅ Need private image storage  
✅ Integrating with ECS/EKS  
✅ Secure container deployment  

👉 ECR = Container image storage layer

---

## ⚖️ ECR vs Docker Hub (IMPORTANT)

| Feature | ECR | Docker Hub |
|--------|-----|------------|
| Integration | AWS-native | External |
| Security | IAM-based | Basic |
| Performance | High (AWS network) | Internet-based |

👉 Prefer ECR for AWS workloads  

---

## ⚡ Features (VERY IMPORTANT)

### 1. Private & Public Repositories
- Private (default)
- Public (optional)

---

### 2. Image Scanning
- Detect vulnerabilities

---

### 3. Lifecycle Policies
- Automatically delete old images

---

### 4. High Availability
- Multi-AZ storage

---

## ⚡ Performance & Scaling

- Fully managed
- Highly scalable
- Optimized for AWS networking

---

## 💸 Cost Optimization

- Pay for:
  - Storage (GB/month)
  - Data transfer

### Reduce cost:
- Use lifecycle policies
- Remove unused images

---

## 🔐 Security

- IAM-based access control
- Encryption at rest (KMS)
- Image scanning for vulnerabilities

---

## 🔄 Integration with Other Services

- [[Amazon ECS]] → container orchestration
- [[Amazon EKS]] → Kubernetes
- [[AWS Fargate]] → serverless containers
- [[AWS CodeBuild]] → CI/CD

---

## 🚀 Real-World Architecture (Pro Level)

### 🐳 Microservices Deployment

1. Build Docker image
2. Push to ECR
3. ECS pulls image
4. Deploy containers behind Load Balancer

👉 End-to-end container pipeline

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. ECR is NOT compute  
👉 It only stores images

🔥 2. Used with ECS/EKS/Fargate  
👉 Always paired

🔥 3. Supports image scanning  
👉 Security feature

🔥 4. Key keyword:
> “Store container images / Docker registry”

👉 Answer = ECR

---

## 🧠 Advanced Architect Insight

ECR is part of **container architecture pipeline**:

Code  
→ Docker build  
→ ECR  
→ ECS/EKS  
→ Production  

---

## 📊 When NOT to Use ECR

❌ Non-container workloads → Use [[Amazon EC2]]  
❌ File storage → Use [[Amazon S3]]  

---

## 🔥 One-Line Summary

👉 ECR = Managed Docker image registry for AWS containers

---

## 🔗 Related Services

- Amazon ECS
- Amazon EKS
- AWS Fargate
- AWS CodeBuild