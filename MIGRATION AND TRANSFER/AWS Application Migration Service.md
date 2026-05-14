# 🧠 AWS Application Migration Service (MGN)

## 🔗 Service Type
#Migration #LiftAndShift #Rehosting #DisasterRecovery

---

## 📌 What is AWS Application Migration Service?

AWS Application Migration Service (MGN) is a service that:

- Migrates applications from on-premises or other clouds to AWS
- Uses lift-and-shift (rehosting) approach

👉 MGN = “Move servers to AWS with minimal changes”

---

## ⚙️ How It Works (Architecture Thinking)

1. Install replication agent on source server

2. Continuous data replication to AWS

3. Create staging environment in AWS

4. Launch test instances

5. Cutover to production

👉 Replicate → Test → Launch → Cutover

---

## 🏗️ Core Concepts (VERY IMPORTANT)

### 1. Replication Agent
- Installed on source servers

---

### 2. Continuous Replication (CRITICAL)
- Keeps data in sync

---

### 3. Staging Area
- Temporary AWS environment

---

### 4. Cutover
- Final migration to production

---

## 🧠 Architectural Logic (Why MGN?)

### When to Choose MGN:

✅ Lift-and-shift migration  
✅ Minimal downtime  
✅ No code changes  
✅ Fast migration  

👉 MGN = Rehosting strategy

---

## ⚖️ MGN vs Other Migration Services (VERY IMPORTANT)

### MGN vs DMS

| Feature | MGN | DMS |
|--------|-----|-----|
| Scope | Full servers | Databases |
| Use case | App migration | DB migration |

---

### MGN vs Snowball

| Feature | MGN | Snowball |
|--------|-----|----------|
| Transfer | Network-based | Physical device |
| Use case | Continuous replication | Large data transfer |

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Continuous Replication
- Near-zero downtime

---

### 2. Automated Conversion
- Converts to AWS-compatible instances

---

### 3. Test Before Cutover
- Validate migration

---

### 4. Non-Disruptive Migration
- No downtime during replication

---

## ⚡ Performance & Scaling

- Scales to multiple servers
- Handles large workloads

---

## 💸 Cost Optimization

- Pay for:
  - Replication infrastructure

### Optimize:
- Stop staging after migration
- Clean unused resources

---

## 🔐 Security

- Encrypted replication
- IAM access control

---

## 🔄 Integration with Other Services

- [[Amazon EC2]] → target instances
- [[Amazon EBS]] → storage
- [[AWS IAM]] → access control
- [[Amazon CloudWatch]] → monitoring

---

## 🚀 Real-World Architecture (Pro Level)

### 🏢 Data Center Migration

On-prem server  
→ MGN replication  
→ AWS staging  
→ Launch EC2  
→ Cutover  

👉 Seamless migration

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. MGN = lift-and-shift ONLY  
👉 No refactoring

🔥 2. Uses continuous replication  
👉 Key feature

🔥 3. Minimal downtime  
👉 Important advantage

🔥 4. Key keyword:
> “Migrate servers / lift-and-shift / minimal downtime”

👉 Answer = AWS Application Migration Service

---

## 🧠 Advanced Architect Insight

MGN enables **rapid cloud adoption strategy**:

On-prem  
→ MGN  
→ AWS  

👉 Fast migration with low risk

---

## 📊 When NOT to Use MGN

❌ Database-only migration → Use [[AWS DMS]]  
❌ Refactoring apps → Use modern services  

---

## 🔥 One-Line Summary

👉 AWS MGN = Lift-and-shift service for migrating servers to AWS

---

## 🔗 Related Services

- AWS DMS
- AWS Snowball
- Amazon EC2
- Amazon EBS