# 🧠 Amazon S3 Glacier

## 🔗 Service Type
#Storage #Archive #ColdStorage #CostOptimization

---

## 📌 What is Amazon S3 Glacier?

Amazon S3 Glacier is a service that:

- Provides low-cost archival storage
- Designed for long-term data retention

👉 Glacier = “Cold storage for archives”

---

## ⚙️ How It Works (Architecture Thinking)

1. Store data in Glacier storage class

2. Data is archived

3. Retrieve when needed:
   - Retrieval takes time

👉 Store → Archive → Retrieve

---

## 🏗️ Storage Classes (VERY IMPORTANT)

### 1. Glacier Instant Retrieval

- Millisecond access
- Higher cost

---

### 2. Glacier Flexible Retrieval (CRITICAL)

- Minutes to hours retrieval

---

### 3. Glacier Deep Archive

- Lowest cost
- Hours retrieval

---

## 🧠 Architectural Logic (VERY IMPORTANT)

### When to Use Glacier:

✅ Long-term backups  
✅ Compliance storage  
✅ Rarely accessed data  
✅ Cost optimization  

👉 Glacier = archive storage

---

## ⚖️ Glacier vs S3 Standard (VERY IMPORTANT)

| Feature | Glacier | S3 Standard |
|--------|--------|-------------|
| Cost | Very low | Higher |
| Access | Slow | Instant |
| Use case | Archive | Active data |

👉 Glacier = cold  
👉 S3 = hot  

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Very Low Cost (CRITICAL)
- Cheapest storage option

---

### 2. Multiple Retrieval Options
- Flexible access speed

---

### 3. Lifecycle Integration
- Move from S3 automatically

---

### 4. High Durability
- Same as S3 (11 9’s)

---

## ⚡ Performance & Scaling

- Scales automatically
- Retrieval latency depends on tier

---

## 💸 Cost Optimization

- Best for long-term storage
- Use lifecycle policies

---

## 🔐 Security (VERY IMPORTANT)

- Encryption support
- IAM policies

---

## 🔄 Integration with Other Services

- [[Amazon S3]] → lifecycle policies
- [[AWS Backup]] → archive backups
- [[AWS Glacier Vault Lock]] → compliance

---

## 🚀 Real-World Architecture (Pro Level)

### 🧊 Backup & Archive System

Data  
→ S3  
→ Lifecycle → Glacier  

👉 Cost-efficient storage

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Glacier = slow retrieval  
👉 Key concept

🔥 2. Cheapest storage  
👉 Important detail

🔥 3. Lifecycle policies move data  
👉 Common scenario

🔥 4. Key keyword:
> “Archive / long-term storage / low cost / infrequent access”

👉 Answer = S3 Glacier

---

## 🧠 Advanced Architect Insight

Glacier enables **cost-efficient data lifecycle**:

Hot data → S3  
Cold data → Glacier  

👉 Optimize cost

---

## 📊 When NOT to Use Glacier

❌ Frequently accessed data → Use [[Amazon S3]]  
❌ Low-latency apps → Avoid  

---

## 🔥 One-Line Summary

👉 Amazon S3 Glacier = Low-cost archival storage for long-term data

---

## 🔗 Related Services

- Amazon S3
- AWS Backup
- AWS KMS