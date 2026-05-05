# 🧠 Amazon Elastic File System (EFS)

## 🔗 Service Type
#Storage #FileStorage #SharedStorage #NFS

---

## 📌 What is Amazon EFS?

Amazon EFS is a service that:

- Provides a shared file system
- Can be accessed by multiple EC2 instances simultaneously

👉 EFS = “Shared file storage for EC2”

---

## ⚙️ How It Works (Architecture Thinking)

1. Create EFS file system

2. Mount on EC2 instances (via NFS)

3. Multiple EC2 instances read/write data

👉 EC2 ↔ EFS ↔ EC2

---

## 🏗️ Core Concepts (VERY IMPORTANT)

### 1. File System (CRITICAL)

- Central storage

---

### 2. Mount Targets

- Created in multiple AZs

---

### 3. NFS Protocol

- Standard file access

---

### 4. Elastic Scaling

- Grows/shrinks automatically

---

## 🧠 Architectural Logic (VERY IMPORTANT)

### When to Use EFS:

✅ Shared storage across EC2  
✅ Linux workloads  
✅ Content management systems  
✅ Web servers  

👉 EFS = shared file system

---

## ⚖️ EFS vs EBS vs S3 (VERY IMPORTANT)

| Feature | EFS | EBS | S3 |
|--------|-----|-----|----|
| Type | File | Block | Object |
| Access | Multiple | Single | Global |
| Use case | Shared files | Disk | Storage |

👉 EFS = shared  
👉 EBS = single disk  
👉 S3 = object storage  

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Shared Access (CRITICAL)
- Multiple instances

---

### 2. Multi-AZ (IMPORTANT)
- High availability

---

### 3. Automatic Scaling
- No capacity planning

---

### 4. Managed Service
- No infrastructure

---

## ⚡ Performance & Scaling

- Scales automatically
- High throughput

---

## 💸 Cost Optimization

- Pay per storage used

---

## 🔐 Security (VERY IMPORTANT)

- Encryption at rest & in transit
- IAM + security groups

---

## 🔄 Integration with Other Services

- [[Amazon EC2]] → compute access
- [[AWS Lambda]] → file system access
- [[Amazon ECS]] → containers

---

## 🚀 Real-World Architecture (Pro Level)

### 🌐 Scalable Web Application

Multiple EC2 instances  
→ Shared EFS  
→ Same files  

👉 Consistent data across servers

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. EFS = multi-AZ  
👉 High availability

🔥 2. Supports multiple EC2  
👉 Key feature

🔥 3. Linux only (mainly)  
👉 Important detail

🔥 4. Key keyword:
> “Shared file system / multiple EC2 / NFS”

👉 Answer = Amazon EFS

---

## 🧠 Advanced Architect Insight

EFS enables **stateless compute + shared storage**:

Compute (EC2)  
→ Shared storage  

👉 Scalable architecture

---

## 📊 When NOT to Use EFS

❌ Single instance → Use [[Amazon EBS]]  
❌ Static content → Use [[Amazon S3]]  

---

## 🔥 One-Line Summary

👉 Amazon EFS = Shared file system for multiple EC2 instances

---

## 🔗 Related Services

- Amazon EC2
- Amazon EBS
- Amazon S3