# 🧠 Amazon EC2 (Elastic Compute Cloud)

## 🔗 Service Type
#Compute #IaaS #VirtualMachines #Scalable

---

## 📌 What is Amazon EC2?

Amazon EC2 provides **resizable virtual servers (instances)** in the cloud.

👉 EC2 = “You control the server”

---

## ⚙️ How It Works (Architecture Thinking)

1. Launch EC2 instance from AMI
2. Choose instance type (CPU, RAM)
3. Configure:
   - Networking ([[Amazon VPC]])
   - Security Groups
   - Storage ([[Amazon EBS]])
4. Deploy application

👉 Full control over OS + runtime

---

## 🏗️ Core Components (VERY IMPORTANT)

### 1. AMI (Amazon Machine Image)
- Pre-configured OS + software
- Used to launch instances

---

### 2. Instance Types

#### Categories:
- General purpose → balanced
- Compute optimized → CPU-heavy
- Memory optimized → RAM-heavy
- Storage optimized → I/O-heavy

👉 Choose based on workload

---

### 3. Storage Options

- [[Amazon EBS]] → persistent block storage
- Instance Store → temporary storage

---

### 4. Networking

- VPC + Subnets
- Security Groups (stateful firewall)
- Elastic IP (static IP)

---

## 🧠 Architectural Logic (Why EC2?)

### When to Choose EC2:

✅ Need full control over OS  
✅ Custom applications  
✅ Long-running workloads  
✅ Lift-and-shift migration  

👉 EC2 = Maximum flexibility

---

## ⚖️ EC2 vs Other Compute Services (VERY IMPORTANT)

### EC2 vs Lambda

| Feature | EC2 | Lambda |
|--------|-----|--------|
| Control | Full | Limited |
| Scaling | Manual/Auto | Automatic |
| Use case | Long-running apps | Event-driven |

👉 EC2 = Control  
👉 Lambda = Serverless  

---

### EC2 vs ECS/Fargate

| Feature | EC2 | ECS/Fargate |
|--------|-----|-------------|
| Level | VM | Containers |
| Management | High | Lower |
| Use case | Traditional apps | Microservices |

---

## ⚡ Scaling (VERY IMPORTANT)

### Vertical Scaling
- Increase instance size

### Horizontal Scaling
- Add more instances (via Auto Scaling)

👉 Horizontal = preferred (high availability)

---

## 💸 Pricing Models (VERY IMPORTANT)

### 1. On-Demand
- Pay per usage

---

### 2. Savings Plans
- Discount for predictable usage

---

### 3. Reserved Instances
- Long-term commitment

---

### 4. Spot Instances (CHEAPEST)
- Up to ~90% cheaper
- Can be interrupted

👉 Best for batch workloads

---

## 🔐 Security

- IAM roles
- Security Groups (stateful)
- NACLs (stateless)
- Key pairs (SSH access)

---

## 🔄 Integration with Other Services

- [[Amazon EBS]] → storage
- [[Amazon S3]] → backup
- [[Elastic Load Balancing]] → traffic distribution
- [[Auto Scaling]] → scaling
- [[Amazon CloudWatch]] → monitoring

---

## 🚀 Real-World Architecture (Pro Level)

### 🌐 Highly Available Web App

1. EC2 instances in multiple AZs
2. Load Balancer distributes traffic
3. Auto Scaling adjusts capacity
4. RDS for database

👉 Fault-tolerant system

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. EC2 requires management  
👉 Patching, scaling, updates

🔥 2. Not serverless  
👉 Compare with Lambda

🔥 3. Spot Instances can be interrupted  
👉 Use for fault-tolerant workloads

🔥 4. Key keyword:
> “Full control over server / custom OS”

👉 Answer = EC2

---

## 🧠 Advanced Architect Insight

EC2 is used in **classic 3-tier architecture**:

Client  
→ Load Balancer  
→ EC2 (App Layer)  
→ Database  

👉 Foundation of many systems

---

## 📊 When NOT to Use EC2

❌ Event-driven → Use [[AWS Lambda]]  
❌ Container-only workloads → Use [[AWS Fargate]]  
❌ No server management → Avoid EC2  

---

## 🔥 One-Line Summary

👉 EC2 = Flexible virtual servers with full control over compute

---

## 🔗 Related Services

- Amazon EBS
- Amazon S3
- Elastic Load Balancing
- Auto Scaling
- AWS Lambda