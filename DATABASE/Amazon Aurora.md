# 🧠 Amazon Aurora

## 🔗 Service Type
#Database #RDS #Relational #HighPerformance

---

## 📌 What is Amazon Aurora?

Amazon Aurora is a **fully managed relational database** compatible with:

- MySQL
- PostgreSQL

👉 Designed for:
- High performance
- High availability
- Scalability

👉 Aurora = “RDS on steroids”

---

## ⚙️ How It Works (Architecture Thinking)

1. Application connects to Aurora cluster

2. Cluster consists of:
   - Writer instance (primary)
   - Multiple read replicas

3. Data stored in **distributed storage layer** across multiple AZs

👉 Compute and storage are separated

---

## 🏗️ Core Architecture (VERY IMPORTANT)

### 1. Cluster

- Writer (1)
- Readers (up to 15 replicas)

---

### 2. Storage Layer (CRITICAL)

- Auto-scales from 10GB to 128TB
- Replicated across 3 AZs (6 copies)

👉 Highly durable

---

### 3. Endpoints

- Writer endpoint → write operations
- Reader endpoint → load-balanced reads

---

## 🧠 Architectural Logic (Why Aurora?)

### When to Choose Aurora:

✅ Need high performance (5x MySQL, 3x PostgreSQL)  
✅ High availability (multi-AZ by default)  
✅ Read-heavy workloads  
✅ Auto-scaling storage  

👉 Aurora = Best relational DB for AWS

---

## ⚖️ Aurora vs RDS vs DynamoDB (VERY IMPORTANT)

### Aurora vs RDS

| Feature | Aurora | RDS |
|--------|--------|-----|
| Performance | Higher | Standard |
| Scaling | Better | Limited |
| Cost | Higher | Lower |

👉 Choose Aurora for performance-critical apps  

---

### Aurora vs DynamoDB

| Feature | Aurora | DynamoDB |
|--------|--------|----------|
| Type | Relational | NoSQL |
| Query | SQL | Key-value |
| Use case | Structured data | Massive scale apps |

---

## ⚡ High Availability (VERY IMPORTANT)

- Multi-AZ by default
- Automatic failover (<30 seconds)

👉 No manual setup needed

---

## ⚡ Scaling

### 1. Read Scaling
- Up to 15 replicas

---

### 2. Storage Scaling
- Automatic

---

### 3. Aurora Serverless (IMPORTANT)

- Auto scales compute
- Pay per use

👉 Serverless = cost-efficient

---

## 💸 Cost Optimization

- More expensive than RDS
- Optimize by:
  - Using Serverless
  - Right-sizing instances
  - Using read replicas

---

## 🔐 Security

- IAM authentication
- Encryption (KMS)
- VPC isolation

---

## 🔄 Integration with Other Services

- [[Amazon EC2]] → application
- [[AWS Lambda]] → serverless integration
- [[Amazon S3]] → backups
- [[Amazon CloudWatch]] → monitoring

---

## 🚀 Real-World Architecture (Pro Level)

### 🌐 High-Traffic Web App

1. App servers (EC2 / ECS)
2. Aurora cluster:
   - Writer for transactions
   - Readers for queries
3. Load balanced reads

👉 Scalable + fault-tolerant DB

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Aurora = multi-AZ by default  
👉 Unlike RDS

🔥 2. Storage auto-scales  
👉 No manual provisioning

🔥 3. Reader endpoint balances load  
👉 Key feature

🔥 4. Key keyword:
> “High performance relational DB with high availability”

👉 Answer = Aurora

---

## 🧠 Advanced Architect Insight

Aurora is used in **high-scale OLTP systems**:

App  
→ Aurora Writer  
→ Aurora Readers  

👉 Separation of read/write workloads

---

## 📊 When NOT to Use Aurora

❌ Simple apps → Use [[Amazon RDS]]  
❌ NoSQL → Use [[Amazon DynamoDB]]  
❌ Low cost priority → Avoid Aurora  

---

## 🔥 One-Line Summary

👉 Aurora = High-performance, scalable relational database with built-in high availability

---

## 🔗 Related Services

- Amazon RDS
- Amazon DynamoDB
- Amazon EC2
- AWS Lambda
- Amazon S3