# 🧠 Amazon EKS Anywhere

## 🔗 Service Type
#Containers #Kubernetes #HybridCloud #Orchestration

---

## 📌 What is Amazon EKS Anywhere?

Amazon EKS Anywhere allows you to run **Kubernetes clusters on your own infrastructure** (on-prem or other environments) using the **same EKS tools and experience**.

👉 EKS Anywhere = “Kubernetes (EKS-style) outside AWS”

---

## ⚙️ How It Works (Architecture Thinking)

1. Install EKS Anywhere on:
   - On-prem servers
   - VMware / bare metal

2. Create Kubernetes cluster

3. Manage cluster using:
   - kubectl
   - EKS tools

4. (Optional) Connect to AWS for:
   - Monitoring
   - Logging

👉 Control + compute both outside AWS

---

## 🏗️ Core Components

### 1. Kubernetes Cluster
- Runs on your infrastructure

---

### 2. EKS Tooling
- Same tooling as AWS EKS

---

### 3. Infrastructure Layer
- VMware / bare metal

---

## 🧠 Architectural Logic (Why EKS Anywhere?)

### When to Choose EKS Anywhere:

✅ Need Kubernetes on-prem  
✅ Want consistent tooling with EKS  
✅ Hybrid or multi-cloud strategy  
✅ Data residency requirements  

👉 EKS Anywhere = On-prem Kubernetes with AWS ecosystem

---

## ⚖️ EKS Anywhere vs Other Services (VERY IMPORTANT)

### EKS Anywhere vs EKS

| Feature | EKS Anywhere | EKS |
|--------|-------------|-----|
| Location | On-prem | AWS |
| Control plane | You manage | AWS manages |
| Use case | Hybrid | Cloud-native |

👉 EKS = managed  
👉 EKS Anywhere = self-managed  

---

### EKS Anywhere vs ECS Anywhere

| Feature | EKS Anywhere | ECS Anywhere |
|--------|-------------|--------------|
| Orchestration | Kubernetes | ECS |
| Complexity | High | Lower |
| Use case | K8s workloads | Simple containers |

---

### EKS Anywhere vs AWS Outposts

| Feature | EKS Anywhere | Outposts |
|--------|-------------|----------|
| Infra | Your hardware | AWS hardware |
| Control | Full control | AWS-managed |
| Services | Kubernetes only | Multiple AWS services |

---

## ⚡ Performance & Scaling

- Depends on your infrastructure
- No AWS-managed scaling

👉 You manage cluster capacity

---

## 💸 Cost Optimization

- No AWS compute cost
- Use existing infrastructure

👉 Pay only for:
- Support (optional)
- External integrations

---

## 🔐 Security

- Kubernetes RBAC
- IAM (for AWS integrations)
- On-prem security controls

---

## 🔄 Integration with Other Services

- [[Amazon ECR]] → container images
- [[Amazon CloudWatch]] → monitoring
- [[AWS IAM]] → identity

---

## 🚀 Real-World Architecture (Pro Level)

### 🏢 Hybrid Kubernetes Platform

1. On-prem Kubernetes via EKS Anywhere
2. Use ECR for images
3. Integrate with AWS monitoring
4. Gradually migrate workloads to EKS

👉 Hybrid Kubernetes strategy

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. EKS Anywhere runs OUTSIDE AWS  
👉 No AWS-managed control plane

🔥 2. You manage everything  
👉 Unlike EKS

🔥 3. Kubernetes only  
👉 Not full AWS services

🔥 4. Key keyword:
> “Run Kubernetes on-prem with EKS tools”

👉 Answer = EKS Anywhere

---

## 🧠 Advanced Architect Insight

EKS Anywhere supports **multi-cloud portability**:

On-Prem  
→ EKS Anywhere  
→ AWS EKS  
→ Other clouds  

👉 Same Kubernetes experience everywhere

---

## 📊 When NOT to Use EKS Anywhere

❌ Want managed Kubernetes → Use [[Amazon EKS]]  
❌ No Kubernetes expertise → Use [[Amazon ECS]]  
❌ Need AWS infra on-prem → Use [[AWS Outposts]]  

---

## 🔥 One-Line Summary

👉 EKS Anywhere = Run Kubernetes clusters on your own infrastructure using EKS tooling

---

## 🔗 Related Services

- Amazon EKS
- Amazon ECS Anywhere
- AWS Outposts
- Amazon ECR
- Amazon CloudWatch