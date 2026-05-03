# 🧠 Amazon EKS Distro (EKS-D)

## 🔗 Service Type
#Containers #Kubernetes #OpenSource #Distribution

---

## 📌 What is Amazon EKS Distro?

Amazon EKS Distro is the **open-source Kubernetes distribution used by Amazon EKS**.

👉 It provides:
- Same Kubernetes version as EKS
- Same binaries and dependencies
- No AWS-managed control plane

👉 EKS-D = “EKS Kubernetes without AWS management”

---

## ⚙️ How It Works (Architecture Thinking)

1. AWS builds Kubernetes distribution (EKS-D)

2. You install it on:
   - On-prem servers
   - VMs
   - Other cloud providers

3. You manage:
   - Control plane
   - Worker nodes

👉 Full control, no AWS automation

---

## 🏗️ Core Components

### 1. Kubernetes Core
- kube-apiserver
- etcd
- scheduler
- controller manager

---

### 2. EKS-Compatible Add-ons
- Networking
- Storage plugins
- Security patches

---

### 3. Version Consistency
- Same version as EKS

---

## 🧠 Architectural Logic (Why EKS Distro?)

### When to Choose EKS-D:

✅ Need Kubernetes without AWS lock-in  
✅ Want full control of cluster  
✅ Build custom Kubernetes platform  
✅ Multi-cloud / edge environments  

👉 EKS-D = DIY Kubernetes (EKS version)

---

## ⚖️ EKS-D vs EKS vs EKS Anywhere (VERY IMPORTANT)

### EKS-D vs EKS

| Feature | EKS-D | EKS |
|--------|------|-----|
| Control plane | You manage | AWS manages |
| Location | Anywhere | AWS cloud |
| Complexity | High | Medium |

---

### EKS-D vs EKS Anywhere

| Feature | EKS-D | EKS Anywhere |
|--------|------|--------------|
| Level | Kubernetes distro | Full solution |
| Setup | Manual | Automated |
| Use case | Advanced users | Easier hybrid |

👉 EKS Anywhere uses EKS-D internally  

---

## ⚡ Performance & Scaling

- Depends entirely on your setup
- No AWS scaling

👉 You manage everything

---

## 💸 Cost Optimization

- Free to use (open-source)
- Pay only for infrastructure

---

## 🔐 Security

- You manage:
  - Patching
  - Upgrades
  - Security

👉 More responsibility

---

## 🔄 Integration with Other Services

- Can integrate with:
  - [[Amazon ECR]] → container images
  - [[Amazon CloudWatch]] → monitoring (optional)
  - [[AWS IAM]] → identity (optional)

---

## 🚀 Real-World Architecture (Pro Level)

### 🌍 Multi-Cloud Kubernetes Platform

1. Use EKS-D across:
   - On-prem
   - AWS
   - Other clouds

2. Maintain consistent Kubernetes version

👉 Avoid vendor lock-in

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. EKS-D is NOT a managed service  
👉 No AWS control plane

🔥 2. It is open-source  
👉 Free to use

🔥 3. Used internally by EKS Anywhere  
👉 Key relationship

🔥 4. Key keyword:
> “Open-source Kubernetes distribution used by EKS”

👉 Answer = EKS Distro

---

## 🧠 Advanced Architect Insight

EKS-D enables **portable Kubernetes architecture**:

Same distro  
→ Any environment  
→ Consistent behavior  

---

## 📊 When NOT to Use EKS-D

❌ Want managed Kubernetes → Use [[Amazon EKS]]  
❌ Want easy hybrid → Use [[Amazon EKS Anywhere]]  
❌ No Kubernetes expertise → Avoid  

---

## 🔥 One-Line Summary

👉 EKS Distro = Open-source Kubernetes distribution used by Amazon EKS

---

## 🔗 Related Services

- Amazon EKS
- Amazon EKS Anywhere
- Amazon ECS
- Amazon ECR