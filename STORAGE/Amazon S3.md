# 🧠 Amazon Simple Storage Service (S3)

## 🔗 Service Type
#Storage #ObjectStorage #Scalable #Core

---

## 📌 What is Amazon S3?

Amazon S3 is a service that:

- Stores data as objects (files)
- Provides unlimited scalable storage

👉 S3 = “Object storage for anything”

---

## ⚙️ How It Works (Architecture Thinking)

1. Create bucket

2. Upload objects (files)

3. Access via:
   - URL
   - API

👉 Bucket → Objects → Access

---

## 🏗️ Core Concepts (VERY IMPORTANT)

### 1. Bucket (CRITICAL)

- Container for objects
- Globally unique name

---

### 2. Object

- File + metadata

---

### 3. Key

- Object name (path)

---

### 4. Versioning

- Keeps multiple versions

---

## 🧠 Architectural Logic (VERY IMPORTANT)

### When to Use S3:

✅ Store files  
✅ Backup & restore  
✅ Static website hosting  
✅ Data lakes  

👉 S3 = universal storage

---

## ⚖️ S3 vs EBS vs EFS (VERY IMPORTANT)

| Feature | S3 | EBS | EFS |
|--------|----|-----|-----|
| Type | Object | Block | File |
| Access | Global | EC2 | Multiple EC2 |
| Use case | Storage | Disk | Shared files |

👉 S3 = object storage  

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Unlimited Storage
- Scales infinitely

---

### 2. High Durability (CRITICAL)
- 99.999999999% (11 9’s)

---

### 3. Storage Classes (IMPORTANT)

- Standard
- Intelligent-Tiering
- Glacier

---

### 4. Lifecycle Policies
- Automate data movement

---

## ⚡ Performance & Scaling

- Automatically scales
- High throughput

---

## 💸 Cost Optimization

- Use storage classes
- Lifecycle policies

---

## 🔐 Security (VERY IMPORTANT)

### 1. Bucket Policies
### 2. IAM Policies
### 3. Encryption (KMS, SSE-S3)
### 4. Block Public Access

---

## 🔄 Integration with Other Services

- [[AWS Lambda]] → event triggers
- [[Amazon CloudFront]] → CDN
- [[AWS Backup]] → storage
- [[Amazon Athena]] → analytics

---

## 🚀 Real-World Architecture (Pro Level)

### 🌐 Static Website Hosting

User  
→ CloudFront  
→ S3 (static files)  

👉 Fully serverless website

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. S3 = object storage  
👉 Not file/block

🔥 2. Global service  
👉 Buckets are global

🔥 3. Strong read-after-write consistency  
👉 Important update

🔥 4. Key keyword:
> “Store files / scalable storage / static hosting”

👉 Answer = Amazon S3

---

## 🧠 Advanced Architect Insight

S3 enables **data-driven architecture**:

Store  
→ Analyze  
→ Process  

👉 Backbone of AWS

---

## 📊 When NOT to Use S3

❌ Low-latency disk → Use [[Amazon EBS]]  
❌ Shared file system → Use [[Amazon EFS]]  

---

## 🔥 One-Line Summary

👉 Amazon S3 = Scalable object storage for any type of data

---

## 🔗 Related Services

- AWS Lambda
- Amazon CloudFront
- Amazon EBS
- Amazon EFS