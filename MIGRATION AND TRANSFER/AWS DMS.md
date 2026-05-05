# 🧠 AWS Database Migration Service (DMS)

## 🔗 Service Type
#Migration #Database #Replication #ETL

---

## 📌 What is AWS DMS?

AWS DMS is a service that:

- Migrates databases to AWS
- Supports continuous replication
- Enables minimal downtime migration

👉 DMS = “Move databases with near-zero downtime”

---

## ⚙️ How It Works (Architecture Thinking)

1. Source database:
   - On-prem / cloud

2. DMS replication instance reads data

3. Transfers data to target DB:
   - [[Amazon RDS]]
   - [[Amazon Aurora]]
   - [[Amazon DynamoDB]]

4. Continuous sync until cutover

👉 Source → Replication → Target

---

## 🏗️ Core Components (VERY IMPORTANT)

### 1. Replication Instance

- Managed compute for migration

---

### 2. Source Endpoint

- Original database

---

### 3. Target Endpoint

- Destination database

---

### 4. Migration Task (CRITICAL)

Types:
- Full load
- CDC (Change Data Capture)
- Full + CDC

---

## 🧠 Architectural Logic (Why DMS?)

### When to Choose DMS:

✅ Database migration  
✅ Minimal downtime  
✅ Continuous replication  
✅ Heterogeneous migration  

👉 DMS = Database migration engine

---

## ⚖️ DMS vs Other Migration Services (VERY IMPORTANT)

### DMS vs MGN

| Feature | DMS | MGN |
|--------|-----|-----|
| Scope | Database | Full server |
| Use case | DB migration | App migration |

---

### DMS vs DataSync

| Feature | DMS | DataSync |
|--------|-----|----------|
| Data type | Databases | Files |
| Use case | Structured data | File transfer |

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Continuous Replication (CDC)

- Sync ongoing changes

---

### 2. Minimal Downtime

- No interruption during migration

---

### 3. Schema Conversion Tool (IMPORTANT)

- Converts DB schema:
  - Oracle → MySQL, etc.

---

### 4. Multi-Target Support

- RDS, Aurora, S3, Redshift

---

## ⚡ Performance & Scaling

- Scales with replication instance size

---

## 💸 Cost Optimization

- Pay for:
  - Replication instance

### Optimize:
- Stop instance after migration
- Use right-sized instance

---

## 🔐 Security

- Encryption in transit
- IAM access control

---

## 🔄 Integration with Other Services

- [[Amazon RDS]] → relational DB
- [[Amazon Aurora]] → high-performance DB
- [[Amazon S3]] → data lake
- [[Amazon Redshift]] → analytics

---

## 🚀 Real-World Architecture (Pro Level)

### 🏢 Database Migration Pipeline

On-prem DB  
→ DMS replication  
→ AWS RDS  

Continuous sync  
→ Cutover  

👉 Zero downtime migration

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. DMS = database ONLY  
👉 Not full server migration

🔥 2. Supports heterogeneous migration  
👉 Key advantage

🔥 3. Uses CDC  
👉 Important concept

🔥 4. Key keyword:
> “Migrate database / minimal downtime / continuous replication”

👉 Answer = AWS DMS

---

## 🧠 Advanced Architect Insight

DMS enables **live migration architecture**:

DB  
→ DMS  
→ AWS DB  

👉 Zero-downtime transition

---

## 📊 When NOT to Use DMS

❌ File transfer → Use [[AWS DataSync]]  
❌ Full app migration → Use [[AWS MGN]]  

---

## 🔥 One-Line Summary

👉 AWS DMS = Migrate databases with minimal downtime using continuous replication

---

## 🔗 Related Services

- AWS Application Migration Service
- AWS DataSync
- Amazon RDS
- Amazon Aurora