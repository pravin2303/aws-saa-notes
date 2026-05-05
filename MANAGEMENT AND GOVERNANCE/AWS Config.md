# 🧠 AWS Config

## 🔗 Service Type
#Governance #Compliance #Monitoring #Audit

---

## 📌 What is AWS Config?

AWS Config is a service that:

- Tracks configuration changes of AWS resources
- Evaluates compliance against rules
- Maintains configuration history

👉 Config = “What changed + Is it compliant?”

---

## ⚙️ How It Works (Architecture Thinking)

1. Resource configuration recorded:
   - EC2
   - S3
   - IAM, etc.

2. Config stores snapshots in:
   - [[Amazon S3]]

3. Evaluate rules:
   - Compliance / non-compliance

4. Optional remediation:
   - [[AWS Lambda]] auto-fix

👉 Track → Evaluate → Fix

---

## 🏗️ Core Concepts (VERY IMPORTANT)

### 1. Configuration Item (CI)
- Snapshot of resource state

---

### 2. Configuration History
- Timeline of changes

---

### 3. Config Rules (CRITICAL)

- Define compliance:
  - “S3 bucket must not be public”

👉 Managed or custom rules

---

### 4. Conformance Packs
- Group of rules for compliance frameworks

---

## 🧠 Architectural Logic (Why AWS Config?)

### When to Choose Config:

✅ Compliance monitoring  
✅ Track configuration changes  
✅ Security auditing  
✅ Governance requirements  

👉 Config = Compliance engine

---

## ⚖️ Config vs CloudTrail vs CloudWatch (VERY IMPORTANT)

| Service | Purpose |
|--------|---------|
| Config | Resource state + compliance |
| CloudTrail | API activity |
| CloudWatch | Metrics/logs |

👉 Config = “What is configured”  
👉 CloudTrail = “Who did it”  
👉 CloudWatch = “What is happening”  

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Continuous Monitoring
- Tracks resource changes

---

### 2. Compliance Evaluation
- Checks against rules

---

### 3. Auto Remediation (IMPORTANT)
- Fix issues using Lambda/SSM

---

### 4. Multi-Account Support
- Central governance

---

## ⚡ High Availability

- Fully managed
- Stores data in S3

---

## 💸 Cost Optimization

- Pay for:
  - Configuration items
  - Rule evaluations

---

## 🔐 Security

- IAM integration
- Encryption via KMS

---

## 🔄 Integration with Other Services

- [[Amazon S3]] → store config history
- [[AWS Lambda]] → remediation
- [[AWS Systems Manager]] → automation
- [[Amazon CloudWatch]] → alerts

---

## 🚀 Real-World Architecture (Pro Level)

### 🔐 Compliance Monitoring System

Config monitors S3 buckets  
→ Rule detects public access  
→ Lambda auto-fixes  

👉 Automated governance

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Config = configuration state  
👉 Not API logs

🔥 2. Rules define compliance  
👉 Key concept

🔥 3. Supports auto-remediation  
👉 Important feature

🔥 4. Key keyword:
> “Track configuration changes / compliance rules”

👉 Answer = AWS Config

---

## 🧠 Advanced Architect Insight

AWS Config enables **continuous compliance architecture**:

Resource  
→ Config  
→ Rule evaluation  
→ Remediation  

👉 Self-healing compliance

---

## 📊 When NOT to Use AWS Config

❌ API auditing → Use [[AWS CloudTrail]]  
❌ Performance monitoring → Use [[Amazon CloudWatch]]  

---

## 🔥 One-Line Summary

👉 AWS Config = Track resource configuration and enforce compliance rules

---

## 🔗 Related Services

- AWS CloudTrail
- Amazon CloudWatch
- AWS Lambda
- AWS Systems Manager