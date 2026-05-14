# 🧠 AWS CloudTrail

## 🔗 Service Type
#Security #Monitoring #Audit #Governance

---

## 📌 What is AWS CloudTrail?

AWS CloudTrail is a service that:

- Records AWS API calls
- Tracks user activity across AWS accounts
- Provides audit logs for security and compliance

👉 CloudTrail = “Who did what in AWS”

---

## ⚙️ How It Works (Architecture Thinking)

1. User / service performs action:
   - Create EC2
   - Delete S3 bucket

2. CloudTrail logs:
   - Who performed action
   - When it happened
   - What was done

3. Logs stored in:
   - [[Amazon S3]]

👉 Full audit trail

---

## 🏗️ Core Concepts (VERY IMPORTANT)

### 1. Event

- Record of an API call

---

### 2. Trails

- Configuration to capture events

---

### 3. Event Types (CRITICAL)

#### Management Events
- Control plane actions (create/delete resources)

---

#### Data Events
- Data-level actions:
  - S3 object access
  - Lambda execution

👉 Data events = more detailed (costly)

---

## 🧠 Architectural Logic (Why CloudTrail?)

### When to Choose CloudTrail:

✅ Audit AWS activity  
✅ Security investigations  
✅ Compliance requirements  
✅ Track API usage  

👉 CloudTrail = Audit & governance

---

## ⚖️ CloudTrail vs CloudWatch vs X-Ray (VERY IMPORTANT)

| Service | Purpose |
|--------|---------|
| CloudTrail | API auditing |
| CloudWatch | Metrics & logs |
| X-Ray | Request tracing |

👉 CloudTrail = “who did it”  
👉 CloudWatch = “what is happening”  
👉 X-Ray = “why it is happening”  

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Multi-Region Logging
- Capture events across regions

---

### 2. Log File Integrity Validation
- Detect tampering

---

### 3. Integration with CloudWatch Logs
- Real-time monitoring

---

### 4. Event History
- View recent events (90 days)

---

## ⚡ High Availability

- Fully managed
- Highly durable (S3 storage)

---

## 💸 Cost Optimization

- Management events → free (basic)
- Data events → charged

---

## 🔐 Security (VERY IMPORTANT)

- IAM integration
- Encryption via KMS
- Secure log storage in S3

---

## 🔄 Integration with Other Services

- [[Amazon S3]] → log storage
- [[Amazon CloudWatch]] → monitoring & alerts
- [[AWS Lambda]] → automated responses
- [[AWS IAM]] → identity tracking

---

## 🚀 Real-World Architecture (Pro Level)

### 🔐 Security Monitoring System

User action → CloudTrail  
→ Logs stored in S3  
→ CloudWatch triggers alert  
→ Lambda responds  

👉 Automated security pipeline

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. CloudTrail = API activity ONLY  
👉 Not performance monitoring

🔥 2. Data events are NOT free  
👉 Important detail

🔥 3. Stores logs in S3  
👉 Key feature

🔥 4. Key keyword:
> “Audit logs / track API calls / compliance”

👉 Answer = CloudTrail

---

## 🧠 Advanced Architect Insight

CloudTrail enables **governance & forensic analysis**:

User action  
→ CloudTrail log  
→ Investigation  

👉 Critical for security

---

## 📊 When NOT to Use CloudTrail

❌ Monitor CPU → Use [[Amazon CloudWatch]]  
❌ Debug microservices → Use [[AWS X-Ray]]  

---

## 🔥 One-Line Summary

👉 CloudTrail = Record and audit AWS API activity

---

## 🔗 Related Services

- Amazon CloudWatch
- AWS X-Ray
- Amazon S3
- AWS IAM