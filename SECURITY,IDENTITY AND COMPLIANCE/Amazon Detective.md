# 🧠 Amazon Detective

## 🔗 Service Type
#Security #Investigation #Analysis #Forensics

---

## 📌 What is Amazon Detective?

Amazon Detective is a service that:

- Helps analyze and investigate security findings
- Provides visual insights into events and relationships

👉 Detective = “Investigate security issues”

---

## ⚙️ How It Works (Architecture Thinking)

1. Collects data from:
   - [[AWS CloudTrail]]
   - [[Amazon VPC]] Flow Logs
   - [[Amazon GuardDuty]]

2. Builds data graph

3. Visualizes relationships:
   - Users
   - Resources
   - Actions

4. Helps analyze root cause

👉 Data → Graph → Analysis → Insight

---

## 🏗️ Core Concepts (VERY IMPORTANT)

### 1. Behavior Graph (CRITICAL)

- Visual representation of activity

---

### 2. Findings Investigation

- Analyze GuardDuty alerts

---

### 3. Data Sources

- CloudTrail
- VPC logs
- GuardDuty

---

### 4. Timeline Analysis

- Track events over time

---

## 🧠 Architectural Logic (VERY IMPORTANT)

### When to Use Amazon Detective:

✅ Investigate security incidents  
✅ Analyze suspicious behavior  
✅ Root cause analysis  
✅ Understand attack patterns  

👉 Detective = security investigation tool

---

## ⚖️ Detective vs GuardDuty vs Security Hub (VERY IMPORTANT)

| Service | Purpose |
|--------|---------|
| GuardDuty | Detect threats |
| Detective | Investigate threats |
| Security Hub | Aggregate findings |

👉 Detective = analysis  

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Visual Graph Analysis
- Easy understanding of relationships

---

### 2. Root Cause Investigation (CRITICAL)
- Identify attack source

---

### 3. Integrated Data Sources
- Multiple logs combined

---

### 4. Timeline Tracking
- See sequence of events

---

## ⚡ Performance & Scaling

- Scales automatically
- Handles large datasets

---

## 💸 Cost Optimization

- Pay for:
  - Data analyzed

---

## 🔐 Security (VERY IMPORTANT)

- Helps strengthen incident response

---

## 🔄 Integration with Other Services

- [[Amazon GuardDuty]] → findings
- [[AWS CloudTrail]] → API logs
- [[Amazon VPC]] → flow logs
- [[AWS Security Hub]] → aggregation

---

## 🚀 Real-World Architecture (Pro Level)

### 🛡️ Security Investigation Workflow

GuardDuty detects threat  
→ Detective analyzes  
→ Security team investigates  

👉 Faster incident response

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Detective = investigation ONLY  
👉 Not detection

🔥 2. Works with GuardDuty  
👉 Important link

🔥 3. Uses visual graphs  
👉 Key feature

🔥 4. Key keyword:
> “Analyze security findings / investigate root cause”

👉 Answer = Amazon Detective

---

## 🧠 Advanced Architect Insight

Detective enables **security forensics**:

Event  
→ Analyze  
→ Understand  
→ Fix  

👉 Deep insight

---

## 📊 When NOT to Use Detective

❌ Detect threats → Use [[Amazon GuardDuty]]  
❌ Aggregate findings → Use [[AWS Security Hub]]  

---

## 🔥 One-Line Summary

👉 Amazon Detective = Analyze and investigate security findings

---

## 🔗 Related Services

- Amazon GuardDuty
- AWS Security Hub
- AWS CloudTrail
- Amazon VPC