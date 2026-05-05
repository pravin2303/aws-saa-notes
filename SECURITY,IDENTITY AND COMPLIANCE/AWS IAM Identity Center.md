# 🧠 AWS IAM Identity Center (formerly AWS SSO)

## 🔗 Service Type
#Security #Identity #SSO #AccessManagement

---

## 📌 What is AWS IAM Identity Center?

AWS IAM Identity Center is a service that:

- Provides Single Sign-On (SSO)
- Manages access to multiple AWS accounts
- Centralizes user authentication

👉 Identity Center = “One login for all AWS accounts & apps”

---

## ⚙️ How It Works (Architecture Thinking)

1. User logs in via Identity Center portal

2. Authenticated via:
   - Built-in directory OR
   - External IdP (Active Directory, SAML)

3. User gets access to:
   - Multiple AWS accounts
   - Applications

👉 User → SSO → Multiple accounts

---

## 🏗️ Core Components (VERY IMPORTANT)

### 1. Identity Source (CRITICAL)

- Identity Center directory OR
- External IdP (AD, Okta)

---

### 2. Permission Sets

- Define access permissions
- Similar to IAM roles

---

### 3. Account Assignments

- Map users/groups → AWS accounts

---

### 4. Access Portal

- Central login UI

---

## 🧠 Architectural Logic (VERY IMPORTANT)

### When to Use IAM Identity Center:

✅ Multiple AWS accounts  
✅ Centralized user management  
✅ Single Sign-On (SSO)  
✅ Enterprise workforce access  

👉 Identity Center = Organization-level access control

---

## ⚖️ IAM vs Identity Center vs Cognito (VERY IMPORTANT)

| Service | Purpose |
|--------|--------|
| IAM | AWS resource access |
| Identity Center | Workforce SSO |
| Cognito | App users |

👉 IAM = low-level  
👉 Identity Center = enterprise users  
👉 Cognito = app users  

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Single Sign-On (SSO)
- One login for all accounts

---

### 2. Centralized Access Control
- Manage permissions centrally

---

### 3. Multi-Account Support (CRITICAL)
- Works with [[AWS Organizations]]

---

### 4. Integration with External IdP
- Active Directory, SAML providers

---

## ⚡ Performance & Scaling

- Fully managed
- Scales across enterprise

---

## 💸 Cost Optimization

- No additional cost for service
- Pay for underlying services

---

## 🔐 Security (VERY IMPORTANT)

- MFA support
- Centralized authentication
- Strong access governance

---

## 🔄 Integration with Other Services

- [[AWS Organizations]] → multi-account setup
- [[AWS IAM]] → permissions
- External IdPs → identity federation

---

## 🚀 Real-World Architecture (Pro Level)

### 🏢 Enterprise Access Management

Employees  
→ Identity Center (SSO)  
→ Access multiple AWS accounts  

👉 Centralized access system

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Identity Center = SSO for workforce  
👉 NOT app users

🔥 2. Uses permission sets (not IAM users)  
👉 Important concept

🔥 3. Works with Organizations  
👉 Multi-account control

🔥 4. Key keyword:
> “Single sign-on / multiple AWS accounts / centralized login”

👉 Answer = IAM Identity Center

---

## 🧠 Advanced Architect Insight

Identity Center enables **enterprise identity architecture**:

Users  
→ SSO  
→ AWS accounts  

👉 Simplified access management

---

## 📊 When NOT to Use Identity Center

❌ App user authentication → Use [[Amazon Cognito]]  
❌ Simple single account → Use IAM  

---

## 🔥 One-Line Summary

👉 AWS IAM Identity Center = Centralized SSO access for multiple AWS accounts

---

## 🔗 Related Services

- AWS IAM
- AWS Organizations
- Amazon Cognito