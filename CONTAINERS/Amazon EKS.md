# 🧠 Amazon EKS (Elastic Kubernetes Service)

## 🔗 Service Type
#Containers #Kubernetes #Orchestration #ManagedService

---

## 📌 What is Amazon EKS?

Amazon EKS is a **fully managed Kubernetes service** that allows you to:

- Run Kubernetes clusters on AWS
- Deploy containerized applications using Kubernetes

👉 EKS = “Managed Kubernetes on AWS”

---

## ⚙️ How It Works (Architecture Thinking)

1. Store container images in [[Amazon ECR]]

2. Deploy Kubernetes cluster via EKS:
   - Control plane managed by AWS

3. Run workloads on:
   - [[Amazon EC2]] (worker nodes)
   - [[AWS Fargate]] (serverless pods)

4. Manage using:
   - kubectl
   - Kubernetes API

👉 AWS manages control plane, you manage workloads

---

## 🏗️ Core Components (VERY IMPORTANT)

### 1. Control Plane
- Managed by AWS
- Handles scheduling, API, cluster state

---

### 2. Worker Nodes
- EC2 instances OR Fargate
- Run containers (pods)

---

### 3. Pods
- Smallest unit in Kubernetes
- Contains containers

---

### 4. Services
- Expose applications
- Load balancing inside cluster

---

## 🧠 Architectural Logic (Why EKS?)

### When to Choose EKS:

✅ Need Kubernetes (industry standard)  
✅ Multi-cloud portability required  
✅ Complex microservices  
✅ Existing Kubernetes expertise  

👉 EKS = Enterprise container orchestration

---

## ⚖️ EKS vs ECS vs Fargate (VERY IMPORTANT)

### EKS vs ECS

| Feature | EKS | ECS |
|--------|-----|-----|
| Orchestration | Kubernetes | AWS-native |
| Complexity | High | Low |
| Portability | High | Low |

👉 ECS = simple  
👉 EKS = flexible + portable  

---

### EKS vs Fargate

| Feature | EKS | Fargate |
|--------|-----|---------|
| Type | Orchestration | Compute |
| Control | High | Low |
| Use case | Complex apps | Simple containers |

---

## ⚡ Scaling & High Availability

- Multi-AZ clusters
- Auto scaling via:
  - Kubernetes HPA
  - EC2 Auto Scaling

👉 Highly scalable system

---

## 💸 Cost Optimization

- Pay for:
  - EKS control plane
  - EC2 / Fargate

### Optimize:
- Use Fargate for simplicity
- Use EC2 for cost savings
- Use Spot Instances

---

## 🔐 Security

- IAM roles (IRSA)
- Kubernetes RBAC
- VPC networking
- Encryption (KMS)

---

## 🔄 Integration with Other Services

- [[Amazon ECR]] → container images
- [[Elastic Load Balancing]] → traffic
- [[AWS IAM]] → authentication
- [[Amazon CloudWatch]] → monitoring

---

## 🚀 Real-World Architecture (Pro Level)

### 🧩 Microservices Platform

1. Images stored in ECR
2. EKS manages cluster
3. Pods run across multiple nodes
4. Load Balancer exposes services

👉 Scalable Kubernetes system

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. EKS = Kubernetes ONLY  
👉 Not simpler than ECS

🔥 2. Control plane managed by AWS  
👉 Worker nodes still yours

🔥 3. More complex than ECS  
👉 Choose only when needed

🔥 4. Key keyword:
> “Kubernetes / portability / multi-cloud”

👉 Answer = EKS

---

## 🧠 Advanced Architect Insight

EKS enables **cloud-agnostic architecture**:

Same Kubernetes  
→ AWS / On-Prem / Other Clouds  

👉 Avoid vendor lock-in

---

## 📊 When NOT to Use EKS

❌ Simple container apps → Use [[Amazon ECS]]  
❌ No Kubernetes expertise → Avoid EKS  
❌ Small workloads → Use [[AWS Fargate]]  

---

## 🔥 One-Line Summary

👉 EKS = Managed Kubernetes service for running containerized applications

---

## 🔗 Related Services

- Amazon ECS
- AWS Fargate
- Amazon ECR
- Amazon EC2
- Elastic Load Balancing