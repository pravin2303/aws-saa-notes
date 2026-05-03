# 🧠 Amazon DocumentDB

## 🔗 Service Type
#Database #NoSQL #DocumentDB #MongoDB

---

## 📌 What is Amazon DocumentDB?

Amazon DocumentDB is a **fully managed NoSQL document database** compatible with:

- MongoDB APIs

👉 Stores data as:
- JSON-like documents (BSON)

👉 DocumentDB = “Managed MongoDB-compatible database”

---

## ⚙️ How It Works (Architecture Thinking)

1. Applications use MongoDB drivers

2. Connect to DocumentDB cluster

3. Data stored in distributed storage layer

👉 Separate compute and storage (like Aurora)

---

## 🏗️ Core Architecture (VERY IMPORTANT)

### 1. Cluster

- 1 primary instance (writes)
- Multiple replicas (reads)

---

### 2. Storage Layer

- Distributed across multiple AZs
- Auto-scaling storage

---

### 3. Endpoints

- Cluster endpoint → writes
- Reader endpoint → read scaling

---

## 🧠 Architectural Logic (Why DocumentDB?)

### When to Choose DocumentDB:

✅ Need MongoDB compatibility  
✅ JSON/document-based data  
✅ Managed NoSQL database  
✅ High availability  

👉 DocumentDB = MongoDB on AWS (managed)

---

## ⚖️ DocumentDB vs DynamoDB vs MongoDB (VERY IMPORTANT)

### DocumentDB vs DynamoDB

| Feature | DocumentDB | DynamoDB |
|--------|------------|----------|
| Model | Document | Key-value |
| Query | Flexible | Limited |
| Use case | JSON apps | High-scale apps |

👉 DynamoDB = scale  
👉 DocumentDB = flexibility  

---

### DocumentDB vs MongoDB (self-managed)

| Feature | DocumentDB | MongoDB |
|--------|------------|---------|
| Management | Fully managed | Self-managed |
| Scaling | Automatic | Manual |
| Ops effort | Low | High |

👉 DocumentDB = easier  

---

## ⚡ High Availability

- Multi-AZ storage
- Automatic failover

👉 Fault-tolerant system

---

## ⚡ Scaling

- Read replicas for scaling
- Storage auto-scales

---

## 💸 Cost Optimization

- Pay for:
  - Instances
  - Storage

### Optimize:
- Use read replicas efficiently
- Right-size instances

---

## 🔐 Security

- IAM authentication
- Encryption (KMS)
- VPC isolation

---

## 🔄 Integration with Other Services

- [[Amazon EC2]] → application layer
- [[AWS Lambda]] → serverless integration
- [[Amazon S3]] → backup
- [[Amazon CloudWatch]] → monitoring

---

## 🚀 Real-World Architecture (Pro Level)

### 🌐 Content Management System

1. App stores JSON documents
2. DocumentDB handles flexible schema
3. Read replicas handle traffic

👉 Scalable document-based system

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. DocumentDB ≠ DynamoDB  
👉 Different NoSQL types

🔥 2. Compatible with MongoDB  
👉 Key keyword

🔥 3. Uses cluster + replicas  
👉 Like Aurora

🔥 4. Key keyword:
> “MongoDB-compatible / document database”

👉 Answer = DocumentDB

---

## 🧠 Advanced Architect Insight

DocumentDB enables **flexible schema applications**:

App  
→ DocumentDB  
→ JSON documents  

👉 No rigid schema required

---

## 📊 When NOT to Use DocumentDB

❌ Key-value high scale → Use [[Amazon DynamoDB]]  
❌ Relational queries → Use [[Amazon Aurora]]  
❌ Complex joins → Avoid  

---

## 🔥 One-Line Summary

👉 DocumentDB = Managed MongoDB-compatible NoSQL database

---

## 🔗 Related Services

- Amazon DynamoDB
- Amazon Aurora
- Amazon EC2
- AWS Lambda
- Amazon S3