# 🧠 Amazon GuardDuty

## 🔗 Service Type
#Security #ThreatDetection #Monitoring #ML

---

## 📌 What is Amazon GuardDuty?

Amazon GuardDuty is a service that:

- Detects threats and suspicious activity
- Uses machine learning + threat intelligence

👉 GuardDuty = “Threat detection system”

---

## ⚙️ How It Works (Architecture Thinking)

1. Collects data from:
   - [[AWS CloudTrail]] → API activity
   - [[Amazon VPC Flow Logs]] → network traffic
   - [[Amazon S3]] logs → data access

2. Analyzes patterns using ML

3. Detects anomalies:
   - Unauthorized access
   - Crypto mining
   - Data exfiltration

4. Generates findings

👉 Logs → Analyze → Detect → Alert

---

## 🏗️ Core Concepts (VERY IMPORTANT)

### 1. Threat Detection (CRITICAL)

- Identifies:
  - Compromised instances
  - Suspicious API calls

---

### 2. Continuous Monitoring

- Always analyzing data

---

### 3. Findings

- Alerts with severity levels

---

### 4. Threat Intelligence

- Uses global threat data

---

## 🧠 Architectural Logic (VERY IMPORTANT)

### When to Use GuardDuty:

✅ Detect attacks  
✅ Monitor AWS environment  
✅ Identify compromised resources  
✅ Security monitoring  

👉 GuardDuty = real-time threat detection

---

## ⚖️ GuardDuty vs Inspector vs Macie (VERY IMPORTANT)

| Service | Purpose |
|--------|---------|
| GuardDuty | Threat detection |
| Inspector | Vulnerabilities |
| Macie | Sensitive data |

👉 GuardDuty = active threats  

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. ML-Based Detection
- Smart anomaly detection

---

### 2. No Agent Required
- Works automatically

---

### 3. Multi-Source Data Analysis
- CloudTrail, VPC logs, S3 logs

---

### 4. Integration with Security Hub
- Central dashboard

---

## ⚡ Performance & Scaling

- Fully managed
- Scales automatically

---

## 💸 Cost Optimization

- Pay for:
  - Events analyzed

---

## 🔐 Security (VERY IMPORTANT)

- Detects threats early
- Improves security posture

---

## 🔄 Integration with Other Services

- [[AWS CloudTrail]] → API logs
- [[Amazon VPC]] → flow logs
- [[Amazon S3]] → access logs
- [[AWS Security Hub]] → aggregation
- [[Amazon EventBridge]] → automation

---

## 🚀 Real-World Architecture (Pro Level)

### 🛡️ Threat Detection System

Logs (CloudTrail + VPC + S3)  
→ GuardDuty  
→ Security Hub  
→ EventBridge → Lambda  

👉 Automated threat response

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. GuardDuty = threat detection ONLY  
👉 Not prevention

🔥 2. Uses logs (no agent)  
👉 Important detail

🔥 3. ML-based analysis  
👉 Key feature

🔥 4. Key keyword:
> “Detect suspicious activity / unusual behavior / compromised resources”

👉 Answer = GuardDuty

---

## 🧠 Advanced Architect Insight

GuardDuty enables **continuous security monitoring**:

Logs  
→ Analyze  
→ Detect threats  

👉 Proactive defense

---

## 📊 When NOT to Use GuardDuty

❌ Vulnerability scanning → Use [[Amazon Inspector]]  
❌ Data classification → Use [[Amazon Macie]]  

---

## 🔥 One-Line Summary

👉 Amazon GuardDuty = Detect threats using logs and machine learning

---

## 🔗 Related Services

- AWS CloudTrail
- Amazon VPC
- Amazon S3
- AWS Security Hub
- Amazon Inspector