# 🧠 AWS Auto Scaling

## 🔗 Service Type
#Compute #Scaling #HighAvailability #CostOptimization

---

## 📌 What is AWS Auto Scaling?

AWS Auto Scaling automatically adjusts **compute capacity** based on demand.

👉 Auto Scaling = “Scale resources up/down automatically”

---

## ⚙️ How It Works (Architecture Thinking)

1. Monitor metrics (CPU, requests, etc.) via [[Amazon CloudWatch]]

2. Apply scaling policy:
   - Scale OUT (add instances)
   - Scale IN (remove instances)

3. Maintain desired capacity

👉 Dynamic infrastructure

---

## 🏗️ Core Components (VERY IMPORTANT)

### 1. Auto Scaling Group (ASG)

- Collection of EC2 instances
- Maintains:
  - Min size
  - Max size
  - Desired capacity

---

### 2. Launch Template

- Defines instance configuration:
  - AMI
  - Instance type
  - Security groups

---

### 3. Scaling Policies (CRITICAL)

#### Target Tracking (MOST COMMON)
- Maintain metric (e.g., CPU = 50%)

---

#### Step Scaling
- Scale in steps based on thresholds

---

#### Scheduled Scaling
- Scale at specific times

---

## 🧠 Architectural Logic (Why Auto Scaling?)

### When to Choose Auto Scaling:

✅ Variable workloads  
✅ High availability requirements  
✅ Cost optimization  
✅ Fault tolerance  

👉 Auto Scaling = Elastic architecture

---

## ⚖️ Horizontal vs Vertical Scaling (VERY IMPORTANT)

### Horizontal Scaling (Scale Out)
- Add/remove instances
- Used by Auto Scaling

---

### Vertical Scaling (Scale Up)
- Increase instance size
- Manual

👉 AWS prefers horizontal scaling

---

## ⚡ High Availability (VERY IMPORTANT)

- Deploy across multiple AZs
- Automatically replaces unhealthy instances

👉 Self-healing architecture

---

## ⚡ Scaling Triggers

- CPU utilization
- Network traffic
- Request count (via Load Balancer)

---

## 💸 Cost Optimization

- Scale in during low demand
- Combine with:
  - Spot Instances
  - Reserved Instances

👉 Pay only for what you use

---

## 🔐 Security

- IAM roles
- Security groups
- VPC integration

---

## 🔄 Integration with Other Services

- [[Elastic Load Balancing]] → distribute traffic
- [[Amazon CloudWatch]] → metrics
- [[Amazon EC2]] → compute

---

## 🚀 Real-World Architecture (Pro Level)

### 🌐 Scalable Web App

User → Load Balancer  
→ Auto Scaling Group (EC2)  
→ Database  

👉 Handles traffic spikes automatically

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Auto Scaling = horizontal scaling  
👉 Not vertical

🔥 2. ASG replaces unhealthy instances  
👉 Self-healing

🔥 3. Target tracking = most common policy  
👉 Easy scaling

🔥 4. Key keyword:
> “Automatically scale EC2 based on demand”

👉 Answer = Auto Scaling

---

## 🧠 Advanced Architect Insight

Auto Scaling enables **elastic cloud architecture**:

Low traffic → fewer instances  
High traffic → more instances  

👉 Efficient + resilient

---

## 📊 When NOT to Use Auto Scaling

❌ Fixed workloads → use static EC2  
❌ Serverless apps → scaling is automatic (Lambda)

---

## 🔥 One-Line Summary

👉 Auto Scaling = Automatically adjust compute capacity based on demand

---

## 🔗 Related Services

- Amazon EC2
- Elastic Load Balancing
- Amazon CloudWatch