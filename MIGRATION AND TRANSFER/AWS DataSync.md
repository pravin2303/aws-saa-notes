# 🧠 AWS DataSync

## 🔗 Service Type
#Migration #DataTransfer #Storage #Sync

---

## 📌 What is AWS DataSync?

AWS DataSync is a service that:

- Transfers large amounts of data
- Between on-premises and AWS
- Or between AWS storage services

👉 DataSync = “Fast, automated data transfer + sync”

---

## ⚙️ How It Works (Architecture Thinking)

1. Install DataSync agent (on-prem)

2. Configure:
   - Source (NFS/SMB)
   - Destination (S3/EFS/FSx)

3. Start transfer task

4. DataSync:
   - Transfers data efficiently
   - Verifies integrity

👉 Source → Agent → AWS Storage

---

## 🏗️ Core Components (VERY IMPORTANT)

### 1. DataSync Agent

- Runs on-premises
- Connects to AWS

---

### 2. Task

- Defines transfer job

---

### 3. Locations

- Source and destination endpoints

---

## 🧠 Architectural Logic (Why DataSync?)

### When to Choose DataSync:

✅ Large-scale data migration  
✅ Continuous data synchronization  
✅ On-prem to AWS transfer  
✅ High-speed transfer  

👉 DataSync = Managed data movement

---

## ⚖️ DataSync vs Other Transfer Services (VERY IMPORTANT)

### DataSync vs Snowball

| Feature | DataSync | Snowball |
|--------|----------|----------|
| Transfer | Network | Physical device |
| Use case | Ongoing sync | One-time large data |

---

### DataSync vs S3 Transfer Acceleration

| Feature | DataSync | Transfer Acceleration |
|--------|----------|----------------------|
| Use case | Bulk migration | Faster uploads |
| Automation | Yes | No |

---

### DataSync vs AWS MGN

| Feature | DataSync | MGN |
|--------|----------|-----|
| Scope | Data | Full servers |
| Use case | File transfer | App migration |

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. High-Speed Transfer
- Optimized network usage

---

### 2. Data Validation (CRITICAL)
- Ensures integrity

---

### 3. Incremental Transfer
- Only changed data moved

---

### 4. Scheduling
- Automate sync tasks

---

## ⚡ Performance & Scaling

- Parallel transfers
- Scales automatically

---

## 💸 Cost Optimization

- Pay for:
  - Data transferred

### Optimize:
- Use incremental sync
- Schedule transfers efficiently

---

## 🔐 Security

- Encryption in transit
- IAM integration

---

## 🔄 Integration with Other Services

- [[Amazon S3]] → storage
- [[Amazon EFS]] → file system
- [[Amazon FSx]] → managed file systems
- [[Amazon CloudWatch]] → monitoring

---

## 🚀 Real-World Architecture (Pro Level)

### 🏢 Data Migration Pipeline

On-prem file server  
→ DataSync agent  
→ S3 / EFS  

👉 Fast, reliable migration

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. DataSync = data transfer ONLY  
👉 Not server migration

🔥 2. Supports continuous sync  
👉 Key advantage

🔥 3. Uses agent for on-prem  
👉 Important detail

🔥 4. Key keyword:
> “Transfer large data / sync files / on-prem to AWS”

👉 Answer = AWS DataSync

---

## 🧠 Advanced Architect Insight

DataSync enables **hybrid storage architectures**:

On-prem  
↔ DataSync  
↔ AWS storage  

👉 Seamless integration

---

## 📊 When NOT to Use DataSync

❌ Full app migration → Use [[AWS MGN]]  
❌ Offline transfer → Use Snowball  

---

## 🔥 One-Line Summary

👉 AWS DataSync = Fast, automated service for transferring and syncing data

---

## 🔗 Related Services

- AWS Snowball
- AWS Application Migration Service
- Amazon S3
- Amazon EFS