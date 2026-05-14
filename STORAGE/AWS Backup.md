# 🧠 AWS Backup

## 🔗 Service Type
#Storage #Backup #DisasterRecovery #Compliance

---

## 📌 What is AWS Backup?

AWS Backup is a service that:

- Centralizes and automates backups
- Across multiple AWS services

👉 AWS Backup = “Unified backup management”

---

## ⚙️ How It Works (Architecture Thinking)

1. Create backup plan:
   - Schedule
   - Retention

2. Assign resources:
   - [[Amazon EC2]] (EBS)
   - [[Amazon RDS]]
   - [[Amazon DynamoDB]]
   - [[Amazon EFS]]

3. Backup is taken automatically

4. Store in backup vault

👉 Plan → Execute → Store → Restore

---

## 🏗️ Core Concepts (VERY IMPORTANT)

### 1. Backup Plan (CRITICAL)

- Defines:
  - Frequency
  - Retention

---

### 2. Backup Vault

- Stores backups securely

---

### 3. Recovery Points

- Snapshots of data

---

### 4. Lifecycle Policies

- Transition/delete backups

---

## 🧠 Architectural Logic (VERY IMPORTANT)

### When to Use AWS Backup:

✅ Centralized backup management  
✅ Compliance requirements  
✅ Automated backups  
✅ Disaster recovery  

👉 AWS Backup = backup automation

---

## ⚖️ AWS Backup vs Snapshots (VERY IMPORTANT)

| Feature | AWS Backup | Snapshots |
|--------|------------|-----------|
| Scope | Multiple services | Single resource |
| Automation | Yes | Manual |
| Centralization | Yes | No |

👉 AWS Backup = enterprise solution  

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Centralized Backup Management
- One place for all backups

---

### 2. Automated Scheduling (CRITICAL)
- No manual work

---

### 3. Cross-Region Backup
- Disaster recovery

---

### 4. Compliance Support
- Retention policies

---

## ⚡ Performance & Scaling

- Scales across resources

---

## 💸 Cost Optimization

- Pay for:
  - Storage
  - Backup usage

---

## 🔐 Security (VERY IMPORTANT)

- Encryption with [[AWS KMS]]
- Access control via IAM

---

## 🔄 Integration with Other Services

- [[Amazon EC2]] → EBS backups
- [[Amazon RDS]] → DB backups
- [[Amazon DynamoDB]] → table backups
- [[Amazon EFS]] → file system backups

---

## 🚀 Real-World Architecture (Pro Level)

### 🛡️ Disaster Recovery System

Resources  
→ AWS Backup  
→ Backup vault  
→ Restore when needed  

👉 Reliable DR strategy

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. AWS Backup = centralized  
👉 Not per service

🔥 2. Uses backup plans  
👉 Important concept

🔥 3. Supports multiple services  
👉 Key advantage

🔥 4. Key keyword:
> “Centralized backup / automated backup / compliance retention”

👉 Answer = AWS Backup

---

## 🧠 Advanced Architect Insight

AWS Backup enables **enterprise-grade backup strategy**:

Plan  
→ Automated backups  
→ Secure storage  

👉 Reliable data protection

---

## 📊 When NOT to Use AWS Backup

❌ Simple snapshot → Use direct snapshot  
❌ Real-time replication → Use other DR tools  

---

## 🔥 One-Line Summary

👉 AWS Backup = Centralized service to automate and manage backups across AWS

---

## 🔗 Related Services

- Amazon EC2
- Amazon RDS
- Amazon DynamoDB
- AWS KMS