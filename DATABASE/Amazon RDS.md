# 🧠 Amazon RDS (Relational Database Service)

## 🔗 Service Type
#Database #Relational #ManagedService #OLTP

---

## 📌 What is Amazon RDS?

Amazon RDS is a **fully managed relational database service** that supports:

- MySQL
- PostgreSQL
- MariaDB
- Oracle
- SQL Server

👉 RDS = “Managed SQL database”

---

## ⚙️ How It Works (Architecture Thinking)

1. Launch DB instance
2. Choose engine (MySQL, PostgreSQL, etc.)
3. Configure:
   - Storage
   - Compute
   - Networking
4. AWS manages:
   - Backups
   - Patching
   - Maintenance

👉 You manage schema + queries only

---

## 🏗️ Core Components (VERY IMPORTANT)

### 1. DB Instance
- Runs database engine

---

### 2. Storage
- EBS-backed storage
- Manual scaling required

---

### 3. Endpoints
- Connect application to DB

---

## 🧠 Architectural Logic (Why RDS?)

### When to Choose RDS:

✅ Need relational database (SQL)  
✅ Structured data  
✅ Transactions (ACID)  
✅ Managed service  

👉 RDS = Default relational DB

---

## ⚖️ RDS vs Aurora vs DynamoDB (VERY IMPORTANT)

### RDS vs Aurora

| Feature | RDS | Aurora |
|--------|-----|--------|
| Performance | Standard | High |
| Scaling | Limited | Better |
| Cost | Lower | Higher |

👉 Aurora = high performance  
👉 RDS = cost-effective  

---

### RDS vs DynamoDB

| Feature | RDS | DynamoDB |
|--------|-----|----------|
| Type | Relational | NoSQL |
| Query | SQL | Key-value |
| Use case | Structured data | Massive scale |

---

## ⚡ High Availability (VERY IMPORTANT)

### Multi-AZ Deployment

- Primary + standby instance
- Automatic failover

👉 Improves availability (not for scaling)

---

## ⚡ Scaling

### 1. Vertical Scaling
- Increase instance size

---

### 2. Read Replicas (IMPORTANT)

- Used for:
  - Read scaling
  - Reporting

👉 NOT for failover (different from Multi-AZ)

---

## 💸 Cost Optimization

- Pay for:
  - Instance
  - Storage

### Optimize:
- Use Reserved Instances
- Use smaller instance sizes
- Use read replicas efficiently

---

## 🔐 Security

- IAM authentication (optional)
- Encryption (KMS)
- VPC isolation
- Security groups

---

## 🔄 Integration with Other Services

- [[Amazon EC2]] → application
- [[AWS Lambda]] → serverless apps
- [[Amazon S3]] → backups
- [[Amazon CloudWatch]] → monitoring

---

## 🚀 Real-World Architecture (Pro Level)

### 🌐 Web Application

1. EC2/ECS → application layer
2. RDS → transactional DB
3. Read replicas → reporting queries

👉 Scalable relational system

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Multi-AZ ≠ read scaling  
👉 Only for failover

🔥 2. Read replicas ≠ failover  
👉 Only for scaling reads

🔥 3. Storage must be provisioned  
👉 Not auto-scaling like Aurora

🔥 4. Key keyword:
> “Relational database / SQL / managed DB”

👉 Answer = RDS

---

## 🧠 Advanced Architect Insight

RDS supports **OLTP workloads**:

App  
→ RDS (transactions)  
→ Read replicas (analytics)  

---

## 📊 When NOT to Use RDS

❌ Massive scale NoSQL → Use [[Amazon DynamoDB]]  
❌ High-performance needs → Use [[Amazon Aurora]]  
❌ Graph relationships → Use [[Amazon Neptune]]  

---

## 🔥 One-Line Summary

👉 RDS = Managed relational database for transactional workloads

---

## 🔗 Related Services

- Amazon Aurora
- Amazon DynamoDB
- Amazon EC2
- AWS Lambda
- Amazon S3