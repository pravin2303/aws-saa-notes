# 🧠 AWS Storage Gateway

## 🔗 Service Type
#Storage #Hybrid #OnPrem #Integration

---

## 📌 What is AWS Storage Gateway?

AWS Storage Gateway is a service that:

- Connects on-premises storage to AWS cloud storage
- Provides hybrid storage solutions

👉 Storage Gateway = “Bridge between on-prem and AWS storage”

---

## ⚙️ How It Works (Architecture Thinking)

1. Deploy gateway on-prem (VM or hardware)

2. Connect to AWS storage:
   - [[Amazon S3]]
   - [[Amazon EBS]]
   - [[Amazon S3 Glacier]]

3. Cache frequently used data locally

4. Store rest in AWS

👉 On-prem → Gateway → AWS storage

---

## 🏗️ Types of Storage Gateway (VERY IMPORTANT — HIGHLY TESTED)

### 1. File Gateway (CRITICAL)

- NFS/SMB interface
- Stores data in S3

👉 Use case:
- File sharing

---

### 2. Volume Gateway

- Block storage interface

Types:
- Cached volumes
- Stored volumes

👉 Use case:
- Backup

---

### 3. Tape Gateway

- Virtual tape library

👉 Use case:
- Backup & archival

---

## 🧠 Architectural Logic (VERY IMPORTANT)

### When to Use Storage Gateway:

✅ Hybrid cloud storage  
✅ Backup to AWS  
✅ Extend on-prem storage  
✅ Disaster recovery  

👉 Storage Gateway = hybrid bridge

---

## ⚖️ Storage Gateway vs DataSync vs Snowball (VERY IMPORTANT)

| Service | Purpose |
|--------|---------|
| Storage Gateway | Hybrid storage |
| DataSync | Data transfer |
| Snowball | Offline transfer |

👉 Gateway = continuous access  

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Hybrid Integration (CRITICAL)
- On-prem + cloud

---

### 2. Local Caching
- Fast access

---

### 3. Multiple Interfaces
- File, block, tape

---

### 4. Backup & DR Support
- Reliable storage

---

## ⚡ Performance & Scaling

- Depends on local cache + network

---

## 💸 Cost Optimization

- Reduce on-prem storage cost
- Pay for cloud storage

---

## 🔐 Security (VERY IMPORTANT)

- Encryption in transit & at rest
- IAM integration

---

## 🔄 Integration with Other Services

- [[Amazon S3]] → storage backend
- [[Amazon S3 Glacier]] → archival
- [[AWS Backup]] → backup automation

---

## 🚀 Real-World Architecture (Pro Level)

### 🏢 Hybrid Backup System

On-prem servers  
→ Storage Gateway  
→ S3 → Glacier  

👉 Cost-effective backup

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Storage Gateway = hybrid  
👉 Not cloud-only

🔥 2. File Gateway uses S3  
👉 Key detail

🔥 3. Tape Gateway = backup  
👉 Important

🔥 4. Key keyword:
> “On-prem + AWS storage / hybrid storage / backup to cloud”

👉 Answer = AWS Storage Gateway

---

## 🧠 Advanced Architect Insight

Storage Gateway enables **hybrid cloud architecture**:

On-prem  
→ Gateway  
→ AWS  

👉 Seamless integration

---

## 📊 When NOT to Use Storage Gateway

❌ One-time transfer → Use DataSync/Snowball  
❌ Cloud-only system → Avoid  

---

## 🔥 One-Line Summary

👉 AWS Storage Gateway = Hybrid storage service connecting on-prem systems to AWS

---

## 🔗 Related Services

- Amazon S3
- Amazon S3 Glacier
- AWS Backup
- AWS DataSync