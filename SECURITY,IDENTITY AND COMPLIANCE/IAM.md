# 🧠 AWS Identity and Access Management (IAM)

## 🔗 Service Type
#Security #Identity #AccessControl #Core

---

## 📌 What is AWS IAM?

AWS IAM is a service that:

- Controls access to AWS resources
- Defines WHO can do WHAT

👉 IAM = “Access control for AWS”

---

## ⚙️ How It Works (Architecture Thinking)

1. Create identity:
   - User / Role

2. Attach policy

3. User/role performs action

4. AWS evaluates:
   - Allow or Deny

👉 Identity + Policy → Access decision

---

## 🏗️ Core Components (VERY IMPORTANT)

### 1. IAM Users

- Individual identities
- Used for:
  - People

---

### 2. IAM Groups

- Collection of users
- Apply permissions once

---

### 3. IAM Roles (CRITICAL)

- Temporary access
- Used by:
  - AWS services
  - Cross-account access

---

### 4. Policies (VERY IMPORTANT)

- JSON documents
- Define permissions

Example:
Allow S3 access

---

## 🧠 Architectural Logic (VERY IMPORTANT)

### When to Use IAM:

✅ Control access to resources  
✅ Secure AWS environment  
✅ Assign permissions  
✅ Enable least privilege  

👉 IAM = security foundation

---

## ⚖️ IAM Users vs Roles (VERY IMPORTANT)

| Feature | User | Role |
|--------|------|------|
| Access | Long-term | Temporary |
| Use case | Humans | Services |

👉 Roles = preferred (best practice)

---

## ⚖️ IAM vs Cognito vs Identity Center

| Service | Purpose |
|--------|---------|
| IAM | AWS access |
| Cognito | App users |
| Identity Center | Workforce SSO |

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Fine-Grained Permissions
- Control actions precisely

---

### 2. Least Privilege (CRITICAL)
- Give minimal access

---

### 3. Role-Based Access
- Temporary credentials

---

### 4. Policy-Based Control
- Flexible permissions

---

## ⚡ Performance & Scaling

- Global service
- Highly scalable

---

## 💸 Cost Optimization

- Free service

---

## 🔐 Security (VERY IMPORTANT)

- MFA support
- Access keys management
- Strong authentication

---

## 🔄 Integration with Other Services

- ALL AWS services:
  - [[Amazon S3]]
  - [[Amazon EC2]]
  - [[AWS Lambda]]

---

## 🚀 Real-World Architecture (Pro Level)

### 🏢 Secure Application Access

User → IAM User  
App → IAM Role  
Service → IAM Role  

👉 Secure access model

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. IAM = global service  
👉 Not region-specific

🔥 2. Roles are temporary  
👉 Best practice

🔥 3. Policies define permissions  
👉 Key concept

🔥 4. Explicit deny overrides allow  
👉 CRITICAL

🔥 5. Key keyword:
> “Control access / permissions / authentication”

👉 Answer = IAM

---

## 🧠 Advanced Architect Insight

IAM enables **least privilege architecture**:

User  
→ Role  
→ Limited access  

👉 Secure system

---

## 📊 When NOT to Use IAM

❌ App users → Use [[Amazon Cognito]]  
❌ Multi-account SSO → Use [[AWS IAM Identity Center]]  

---

## 🔥 One-Line Summary

👉 AWS IAM = Control access to AWS resources using users, roles, and policies

---

## 🔗 Related Services

- Amazon Cognito
- AWS IAM Identity Center
- AWS KMS