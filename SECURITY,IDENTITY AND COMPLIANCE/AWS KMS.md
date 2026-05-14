# 🧠 AWS Key Management Service (KMS)

## 🔗 Service Type
#Security #Encryption #KeyManagement #DataProtection

---

## 📌 What is AWS KMS?

AWS KMS is a service that:

- Creates and manages encryption keys
- Controls how data is encrypted and decrypted

👉 KMS = “Central key management for AWS”

---

## ⚙️ How It Works (Architecture Thinking)

1. Create KMS key

2. Use key to:
   - Encrypt data
   - Decrypt data

3. Services integrate with KMS

👉 Data → Encrypt → Store securely

---

## 🏗️ Core Concepts (VERY IMPORTANT)

### 1. KMS Keys (CMKs)

Types:
- AWS-managed keys
- Customer-managed keys (CRITICAL)

---

### 2. Envelope Encryption (CRITICAL)

- Data encrypted using:
  - Data key
- Data key encrypted using:
  - KMS key

👉 Secure + efficient

---

### 3. Key Policies

- Control access to keys

---

### 4. Automatic Key Rotation

- Enabled for customer-managed keys

---

## 🧠 Architectural Logic (VERY IMPORTANT)

### When to Use KMS:

✅ Encrypt data at rest  
✅ Manage encryption keys  
✅ Compliance requirements  
✅ Secure AWS services  

👉 KMS = encryption backbone

---

## ⚖️ AWS-managed vs Customer-managed Keys (VERY IMPORTANT)

| Feature | AWS-managed | Customer-managed |
|--------|------------|------------------|
| Control | Limited | Full |
| Rotation | Automatic | Optional |
| Visibility | Limited | Full |

👉 Customer-managed = more control  

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Centralized Key Management
- One place for all keys

---

### 2. Integrated Encryption
- Works with many AWS services

---

### 3. Secure Key Storage
- Hardware Security Modules (HSM)

---

### 4. Fine-Grained Access Control
- IAM + key policies

---

## ⚡ Performance & Scaling

- Highly scalable
- Low latency

---

## 💸 Cost Optimization

- Pay per:
  - API calls
  - Key usage

---

## 🔐 Security (VERY IMPORTANT)

- Keys never leave AWS
- Encrypted storage
- IAM control

---

## 🔄 Integration with Other Services

- [[Amazon S3]] → object encryption
- [[Amazon EBS]] → volume encryption
- [[Amazon RDS]] → database encryption
- [[AWS Lambda]] → environment variables

---

## 🚀 Real-World Architecture (Pro Level)

### 🔐 Secure Data Storage

App  
→ KMS encrypts data  
→ Stored in S3 / RDS  

👉 Secure-by-design system

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. KMS manages keys ONLY  
👉 Not storage

🔥 2. Uses envelope encryption  
👉 Key concept

🔥 3. Customer-managed keys give control  
👉 Important distinction

🔥 4. Key keyword:
> “Encrypt data / manage keys / compliance”

👉 Answer = AWS KMS

---

## 🧠 Advanced Architect Insight

KMS enables **secure-by-default architecture**:

Data  
→ Encrypted  
→ Stored  

👉 Compliance-ready

---

## 📊 When NOT to Use KMS

❌ Simple encryption without AWS integration  
❌ Need full HSM control → Use CloudHSM  

---

## 🔥 One-Line Summary

👉 AWS KMS = Managed service to create and control encryption keys

---

## 🔗 Related Services

- Amazon S3
- Amazon RDS
- AWS CloudHSM
- AWS IAM