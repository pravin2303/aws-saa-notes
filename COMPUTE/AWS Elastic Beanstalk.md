# 🧠 AWS Elastic Beanstalk

## 🔗 Service Type
#Compute #PaaS #Deployment #ManagedService

---

## 📌 What is AWS Elastic Beanstalk?

AWS Elastic Beanstalk is a **Platform as a Service (PaaS)** that allows you to:

- Deploy applications quickly
- Manage infrastructure automatically

👉 You upload code → AWS handles:
- EC2
- Auto Scaling
- Load Balancer
- Monitoring

---

## ⚙️ How It Works (Architecture Thinking)

1. Upload application code
2. Beanstalk provisions:
   - [[Amazon EC2]]
   - [[Amazon EC2 Auto Scaling]]
   - [[Elastic Load Balancing]]
3. Deploys application
4. Monitors via [[Amazon CloudWatch]]

👉 Fully managed deployment pipeline

---

## 🏗️ Core Components

### 1. Application
- Logical container for your app

---

### 2. Environment (VERY IMPORTANT)

- Web Server Environment
  - For HTTP apps
- Worker Environment
  - For background processing

---

### 3. Platform
- Pre-configured runtime:
  - Node.js
  - Python
  - Java
  - Docker

---

## 🧠 Architectural Logic (Why Elastic Beanstalk?)

### When to Choose Beanstalk:

✅ Want to deploy quickly  
✅ Don’t want to manage infrastructure  
✅ Traditional web applications  
✅ Need auto scaling + load balancing  

👉 Beanstalk = “Managed EC2 platform”

---

## ⚖️ Beanstalk vs Other Services (VERY IMPORTANT)

### Beanstalk vs EC2

| Feature | Beanstalk | EC2 |
|--------|----------|-----|
| Management | Automated | Manual |
| Control | Moderate | Full |
| Use case | App deployment | Custom infra |

👉 EC2 = control  
👉 Beanstalk = convenience  

---

### Beanstalk vs Lambda

| Feature | Beanstalk | Lambda |
|--------|----------|--------|
| Type | PaaS | Serverless |
| Use case | Web apps | Event-driven |
| Scaling | Managed | Fully automatic |

---

## ⚡ Deployment Options (IMPORTANT)

### 1. All-at-once
- Fast but risky

### 2. Rolling
- Gradual deployment

### 3. Blue/Green (VERY IMPORTANT)
- Deploy new version separately
- Switch traffic

👉 Zero downtime deployment

---

## ⚡ Performance & Scaling

- Uses Auto Scaling automatically
- Integrates with Load Balancer

👉 Handles traffic spikes

---

## 💸 Cost Optimization

- No additional cost for Beanstalk
- Pay only for:
  - EC2
  - Load Balancer
  - Storage

👉 Optimize using:
- Right instance types
- Auto Scaling

---

## 🔐 Security

- IAM roles
- Security groups
- HTTPS via Load Balancer

---

## 🔄 Integration with Other Services

- [[Amazon EC2]] → compute
- [[Elastic Load Balancing]] → traffic
- [[Amazon RDS]] → database
- [[Amazon S3]] → storage
- [[Amazon CloudWatch]] → monitoring

---

## 🚀 Real-World Architecture (Pro Level)

### 🌐 Web Application Deployment

1. Developer uploads code
2. Beanstalk provisions:
   - EC2 + Auto Scaling
   - Load Balancer
3. App deployed across multiple AZs

👉 Production-ready setup with minimal effort

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Beanstalk is NOT serverless  
👉 Uses EC2 underneath

🔥 2. Limited customization  
👉 Compared to EC2

🔥 3. Supports Blue/Green deployment  
👉 Important exam topic

🔥 4. Key keyword:
> “Deploy application without managing infrastructure”

👉 Answer = Elastic Beanstalk

---

## 🧠 Advanced Architect Insight

Beanstalk is used for **rapid application deployment**:

Code  
→ Beanstalk  
→ EC2 + ALB + ASG  

👉 Quick production setup

---

## 📊 When NOT to Use Beanstalk

❌ Need full control → Use [[Amazon EC2]]  
❌ Event-driven → Use [[AWS Lambda]]  
❌ Microservices containers → Use [[Amazon ECS]] / [[AWS Fargate]]  

---

## 🔥 One-Line Summary

👉 Elastic Beanstalk = PaaS for deploying and managing web applications easily

---

## 🔗 Related Services

- Amazon EC2
- Auto Scaling
- Elastic Load Balancing
- Amazon RDS
- AWS Lambda