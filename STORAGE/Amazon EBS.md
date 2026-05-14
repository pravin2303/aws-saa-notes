# 🧠 Amazon Elastic Block Store (EBS)

## 🔗 Service Type
#Storage #BlockStorage #EC2 #Persistence

---

## 📌 What is Amazon EBS?

Amazon EBS is a service that:

- Provides block storage volumes for EC2 instances
- Acts like a virtual hard disk

👉 EBS = “Disk for EC2”

---

## ⚙️ How It Works (Architecture Thinking)

1. Create EBS volume

2. Attach to:
   - [[Amazon EC2]]

3. EC2 reads/writes data

👉 EC2 ↔ EBS

---

## 🏗️ Core Concepts (VERY IMPORTANT)

### 1. Volume (CRITICAL)

- Storage unit
- Types:
  - gp3 (general purpose)
  - io1/io2 (high performance)

---

### 2. AZ Bound (IMPORTANT)

- Volume exists in ONE Availability Zone

---

### 3. Snapshot

- Backup stored in [[Amazon S3]]

---

### 4. Detach & Attach

- Move volume between instances (same AZ)

---

## 🧠 Architectural Logic (VERY IMPORTANT)

### When to Use EBS:

✅ Persistent storage for EC2  
✅ High-performance disk  
✅ Databases  
✅ Boot volume  

👉 EBS = block storage

---

## ⚖️ EBS vs S3 vs EFS (VERY IMPORTANT)

| Feature | EBS | S3 | EFS |
|--------|-----|----|-----|
| Type | Block | Object | File |
| Use case | EC2 disk | Storage | Shared files |
| Access | Single instance | Global | Multiple |

👉 EBS = disk  
👉 S3 = object storage  
👉 EFS = shared file system  

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Persistent Storage
- Data survives instance stop

---

### 2. High Performance
- Low latency

---

### 3. Snapshots (CRITICAL)
- Backup + restore

---

### 4. Encryption
- Uses [[AWS KMS]]

---

## ⚡ Performance & Scaling

- Scale by changing volume type/size

---

## 💸 Cost Optimization

- Pay for:
  - Storage size
  - IOPS

---

## 🔐 Security (VERY IMPORTANT)

- Encryption at rest
- IAM access control

---

## 🔄 Integration with Other Services

- [[Amazon EC2]] → compute
- [[Amazon S3]] → snapshot storage
- [[AWS KMS]] → encryption

---

## 🚀 Real-World Architecture (Pro Level)

### 💾 EC2 Application Storage

EC2  
→ EBS (OS + data)  
→ Snapshot backup  

👉 Persistent system

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. EBS = AZ-specific  
👉 Cannot directly attach across AZ

🔥 2. Single instance (mostly)  
👉 Not shared (except special cases)

🔥 3. Snapshots stored in S3  
👉 Key concept

🔥 4. Key keyword:
> “Attach storage to EC2 / block storage / persistent disk”

👉 Answer = Amazon EBS

---

## 🧠 Advanced Architect Insight

EBS enables **stateful EC2 architecture**:

Compute  
+ Storage  
→ Persistent system  

👉 Reliable workloads

---

## 📊 When NOT to Use EBS

❌ Shared storage → Use [[Amazon EFS]]  
❌ Static files → Use [[Amazon S3]]  

---

## 🔥 One-Line Summary

👉 Amazon EBS = Persistent block storage for EC2 instances

---

## 🔗 Related Services

- Amazon EC2
- Amazon S3
- Amazon EFS
- AWS KMS