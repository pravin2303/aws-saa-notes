# 🧠 AWS Service Catalog

## 🔗 Service Type
#Governance #Provisioning #SelfService #Standardization

---

## 📌 What is AWS Service Catalog?

AWS Service Catalog is a service that allows organizations to:

- Create and manage approved AWS resources
- Provide users with self-service access to these resources

👉 Service Catalog = “Controlled self-service provisioning”

---

## ⚙️ How It Works (Architecture Thinking)

1. Admin defines products:
   - CloudFormation templates

2. Organize into portfolios

3. Grant access to users

4. Users launch resources from catalog

👉 Admin controls → Users deploy safely

---

## 🏗️ Core Concepts (VERY IMPORTANT)

### 1. Product

- Predefined resource (e.g., EC2 setup)

---

### 2. Portfolio

- Collection of products

---

### 3. Launch Constraints (CRITICAL)

- Control:
  - Who can launch
  - How resources are created

---

### 4. Provisioning

- Launch resources via templates

---

## 🧠 Architectural Logic (Why Service Catalog?)

### When to Choose Service Catalog:

✅ Standardized infrastructure  
✅ Controlled deployments  
✅ Enterprise governance  
✅ Self-service for teams  

👉 Service Catalog = Safe provisioning layer

---

## ⚖️ Service Catalog vs CloudFormation (VERY IMPORTANT)

| Feature | Service Catalog | CloudFormation |
|--------|----------------|----------------|
| Purpose | Controlled access | Resource creation |
| Users | End users | DevOps/admins |
| Control | High | Moderate |

👉 CloudFormation = build infra  
👉 Service Catalog = control access  

---

## ⚖️ Service Catalog vs Control Tower

| Feature | Service Catalog | Control Tower |
|--------|----------------|--------------|
| Scope | Resource provisioning | Account governance |
| Use case | Standard apps | Multi-account setup |

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Standardized Deployments
- Pre-approved configurations

---

### 2. Access Control
- IAM-based permissions

---

### 3. Version Control
- Manage product versions

---

### 4. Cost & Compliance Control
- Prevent misuse

---

## ⚡ Performance & Scaling

- Scales with CloudFormation
- Supports large organizations

---

## 💸 Cost Optimization

- No cost for Service Catalog
- Helps avoid misconfigured resources

---

## 🔐 Security (VERY IMPORTANT)

- IAM integration
- Launch constraints enforce policies

---

## 🔄 Integration with Other Services

- [[AWS CloudFormation]] → provisioning engine
- [[AWS Organizations]] → multi-account access
- [[AWS IAM]] → permissions
- [[AWS Config]] → compliance tracking

---

## 🚀 Real-World Architecture (Pro Level)

### 🏢 Enterprise Self-Service Platform

Admin defines:
- EC2 templates
- VPC templates

Users:
- Deploy via Service Catalog

👉 Controlled + scalable deployments

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Service Catalog = NOT infrastructure creation  
👉 Uses CloudFormation internally

🔥 2. Focus on governance  
👉 Controlled access

🔥 3. Users launch pre-approved resources  
👉 Key concept

🔥 4. Key keyword:
> “Pre-approved resources / self-service / controlled provisioning”

👉 Answer = AWS Service Catalog

---

## 🧠 Advanced Architect Insight

Service Catalog enables **controlled DevOps environments**:

Admin  
→ Define templates  
→ Users deploy safely  

👉 Balance between flexibility & control

---

## 📊 When NOT to Use Service Catalog

❌ Full automation → Use [[AWS CloudFormation]]  
❌ Simple setup → Use Console/CLI  

---

## 🔥 One-Line Summary

👉 AWS Service Catalog = Provide users access to pre-approved AWS resources

---

## 🔗 Related Services

- AWS CloudFormation
- AWS Organizations
- AWS IAM
- AWS Config