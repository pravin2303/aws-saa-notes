# 🧠 AWS Resource Access Manager (RAM)

## 🔗 Service Type
#Governance #Sharing #MultiAccount #Networking

---

## 📌 What is AWS RAM?

AWS Resource Access Manager (RAM) is a service that:

- Allows you to share AWS resources across accounts
- Without duplicating resources

👉 RAM = “Share resources across AWS accounts”

---

## ⚙️ How It Works (Architecture Thinking)

1. Resource owner shares resource

2. Specifies:
   - Accounts
   - Organizational Units (OUs)

3. Target account accesses shared resource

👉 Owner → Share → Consumer

---

## 🏗️ Core Concepts (VERY IMPORTANT)

### 1. Resource Share

- Collection of resources to share

---

### 2. Principals (CRITICAL)

- Who gets access:
  - AWS accounts
  - OUs

---

### 3. Supported Resources

Examples:
- VPC subnets
- Transit Gateway
- Route 53 Resolver rules

---

## 🧠 Architectural Logic (VERY IMPORTANT)

### When to Use AWS RAM:

✅ Multi-account architecture  
✅ Share network resources  
✅ Avoid duplication  
✅ Centralized infrastructure  

👉 RAM = resource sharing layer

---

## ⚖️ RAM vs IAM vs Organizations (VERY IMPORTANT)

| Service | Purpose |
|--------|---------|
| RAM | Share resources |
| IAM | Control access |
| Organizations | Manage accounts |

👉 RAM = sharing  
👉 IAM = permissions  

---

## ⚖️ RAM vs VPC Peering

| Feature | RAM | VPC Peering |
|--------|-----|-------------|
| Use case | Share resource | Connect networks |
| Scope | Specific resource | Entire VPC |

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Cross-Account Sharing
- Share without copying

---

### 2. Integration with Organizations
- Share across OUs

---

### 3. Centralized Resource Management
- One resource, many accounts

---

### 4. Supported Resource Types
- Networking services (IMPORTANT)

---

## ⚡ Performance & Scaling

- Highly scalable
- Supports many accounts

---

## 💸 Cost Optimization

- Avoid duplicate resources
- Reduce cost

---

## 🔐 Security (VERY IMPORTANT)

- Controlled sharing
- IAM + resource policies

---

## 🔄 Integration with Other Services

- [[AWS Organizations]] → account management
- [[Amazon VPC]] → subnet sharing
- [[AWS Transit Gateway]] → shared networking

---

## 🚀 Real-World Architecture (Pro Level)

### 🏢 Shared Networking Architecture

Central networking account  
→ Shares VPC subnets via RAM  
→ Multiple application accounts use them  

👉 Centralized network design

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. RAM = resource sharing ONLY  
👉 Not access control

🔥 2. Works across accounts  
👉 Key feature

🔥 3. Often used with Organizations  
👉 Important context

🔥 4. Key keyword:
> “Share resources across accounts / avoid duplication”

👉 Answer = AWS RAM

---

## 🧠 Advanced Architect Insight

RAM enables **centralized infrastructure architecture**:

Shared resource  
→ Multiple accounts  
→ Efficient design  

👉 Enterprise-ready setup

---

## 📊 When NOT to Use RAM

❌ Connect VPCs → Use [[AWS Transit Gateway]]  
❌ Control permissions → Use [[AWS IAM]]  

---

## 🔥 One-Line Summary

👉 AWS RAM = Share AWS resources across multiple accounts

---

## 🔗 Related Services

- AWS Organizations
- Amazon VPC
- AWS Transit Gateway
- AWS IAM