# 🧠 Amazon Inspector

## 🔗 Service Type
#Security #Vulnerability #Scanning #Compliance

---

## 📌 What is Amazon Inspector?

Amazon Inspector is a service that:

- Automatically scans AWS workloads
- Identifies vulnerabilities and security issues

👉 Inspector = “Find vulnerabilities in resources”

---

## ⚙️ How It Works (Architecture Thinking)

1. Inspector scans:
   - [[Amazon EC2]] instances
   - Container images (ECR)

2. Checks for:
   - CVEs (Common Vulnerabilities)
   - Misconfigurations

3. Generates findings

4. Sends results to:
   - [[AWS Security Hub]]

👉 Resource → Scan → Detect → Report

---

## 🏗️ Core Concepts (VERY IMPORTANT)

### 1. Vulnerability Scanning (CRITICAL)

- Detect:
  - OS vulnerabilities
  - Software issues

---

### 2. Continuous Monitoring

- Ongoing scans

---

### 3. Findings

- Alerts for vulnerabilities

---

### 4. Risk Scoring

- Prioritizes issues

---

## 🧠 Architectural Logic (VERY IMPORTANT)

### When to Use Inspector:

✅ Scan EC2 instances  
✅ Scan container images  
✅ Detect vulnerabilities  
✅ Improve security posture  

👉 Inspector = vulnerability detection

---

## ⚖️ Inspector vs GuardDuty vs Macie (VERY IMPORTANT)

| Service | Purpose |
|--------|---------|
| Inspector | Vulnerabilities |
| GuardDuty | Threat detection |
| Macie | Sensitive data |

👉 Inspector = weaknesses  

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Automated Scanning
- Continuous analysis

---

### 2. CVE Detection (CRITICAL)
- Known vulnerabilities

---

### 3. Container Security
- Scans ECR images

---

### 4. Integration with Security Hub
- Centralized alerts

---

## ⚡ Performance & Scaling

- Scales automatically
- Real-time scanning

---

## 💸 Cost Optimization

- Pay per:
  - Resources scanned

---

## 🔐 Security (VERY IMPORTANT)

- Identifies risks before exploitation

---

## 🔄 Integration with Other Services

- [[Amazon EC2]] → compute scanning
- [[Amazon ECR]] → container scanning
- [[AWS Security Hub]] → aggregation
- [[Amazon EventBridge]] → automation

---

## 🚀 Real-World Architecture (Pro Level)

### 🛡️ Secure Infrastructure

EC2 / ECR  
→ Inspector scans  
→ Findings  
→ Security Hub  

👉 Vulnerability management

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Inspector = vulnerability scanning  
👉 NOT threat detection

🔥 2. Works with EC2 & ECR  
👉 Key detail

🔥 3. Continuous scanning  
👉 Important feature

🔥 4. Key keyword:
> “Scan for vulnerabilities / CVEs / security assessment”

👉 Answer = Amazon Inspector

---

## 🧠 Advanced Architect Insight

Inspector enables **proactive security**:

Scan  
→ Detect  
→ Fix  

👉 Reduce risk

---

## 📊 When NOT to Use Inspector

❌ Detect active attacks → Use [[Amazon GuardDuty]]  
❌ Find sensitive data → Use [[Amazon Macie]]  

---

## 🔥 One-Line Summary

👉 Amazon Inspector = Automatically scan workloads for vulnerabilities

---

## 🔗 Related Services

- Amazon EC2
- Amazon ECR
- AWS Security Hub
- Amazon GuardDuty