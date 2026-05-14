# 🧠 AWS Directory Service

## 🔗 Service Type
#Security #Identity #Directory #ActiveDirectory

---

## 📌 What is AWS Directory Service?

AWS Directory Service is a service that:

- Provides managed Microsoft Active Directory (AD)
- Enables authentication and directory-based access

👉 Directory Service = “Active Directory in AWS”

---

## ⚙️ How It Works (Architecture Thinking)

1. Deploy directory in AWS

2. Connect users/applications

3. Authenticate via directory

4. Integrate with AWS services

👉 User → Directory → Authentication

---

## 🏗️ Directory Types (VERY IMPORTANT — HIGHLY TESTED)

### 1. AWS Managed Microsoft AD (MOST IMPORTANT)

- Full Active Directory
- Managed by AWS

👉 Use case:
- Enterprise apps
- Windows workloads

---

### 2. AD Connector

- Proxy to on-prem AD

👉 Use case:
- Hybrid environment

---

### 3. Simple AD

- Lightweight directory (basic)

👉 Use case:
- Small apps

---

## 🧠 Architectural Logic (VERY IMPORTANT)

### When to Use Directory Service:

✅ Windows-based authentication  
✅ Active Directory integration  
✅ Domain join EC2 instances  
✅ Enterprise identity management  

👉 Directory Service = AD integration

---

## ⚖️ Directory Service vs IAM vs Identity Center (VERY IMPORTANT)

| Service | Purpose |
|--------|---------|
| IAM | AWS resource access |
| Directory Service | AD-based authentication |
| Identity Center | SSO across accounts |

👉 Directory = enterprise identity  

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Managed Active Directory
- No infrastructure management

---

### 2. Domain Join (CRITICAL)
- EC2 instances join domain

---

### 3. Integration with AWS Services
- Works with:
  - EC2
  - RDS (SQL Server)
  - WorkSpaces

---

### 4. Hybrid Support
- Connect to on-prem AD

---

## ⚡ Performance & Scaling

- Highly available
- Multi-AZ deployment

---

## 💸 Cost Optimization

- Pay for directory instances

---

## 🔐 Security (VERY IMPORTANT)

- Secure authentication
- Integration with IAM

---

## 🔄 Integration with Other Services

- [[Amazon EC2]] → domain join
- [[Amazon RDS]] → Windows auth
- [[AWS IAM Identity Center]] → SSO
- [[Amazon WorkSpaces]] → virtual desktops

---

## 🚀 Real-World Architecture (Pro Level)

### 🏢 Enterprise Windows Environment

Employees  
→ Active Directory  
→ EC2 Windows servers  

👉 Centralized identity system

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Managed Microsoft AD = full AD  
👉 Most important

🔥 2. AD Connector = proxy  
👉 No directory stored in AWS

🔥 3. Used for Windows workloads  
👉 Key use case

🔥 4. Key keyword:
> “Active Directory / domain join / Windows authentication”

👉 Answer = AWS Directory Service

---

## 🧠 Advanced Architect Insight

Directory Service enables **enterprise identity integration**:

Users  
→ AD  
→ AWS resources  

👉 Hybrid identity solution

---

## 📊 When NOT to Use Directory Service

❌ App user login → Use [[Amazon Cognito]]  
❌ Simple AWS access → Use [[AWS IAM]]  

---

## 🔥 One-Line Summary

👉 AWS Directory Service = Managed Active Directory for authentication in AWS

---

## 🔗 Related Services

- AWS IAM
- AWS IAM Identity Center
- Amazon EC2
- Amazon WorkSpaces