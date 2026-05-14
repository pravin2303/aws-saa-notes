# 🧠 AWS CLI (Command Line Interface)

## 🔗 Service Type
#DeveloperTools #Automation #CLI #DevOps

---

## 📌 What is AWS CLI?

AWS CLI is a **command-line tool** that allows you to:

- Interact with AWS services
- Automate tasks
- Manage resources from terminal

👉 CLI = “Control AWS using commands”

---

## ⚙️ How It Works (Architecture Thinking)

1. Install AWS CLI

2. Configure credentials:
   - Access Key
   - Secret Key
   - Region

3. Run commands:

Example:
aws s3 ls

👉 CLI → AWS API → Service

---

## 🏗️ Core Concepts (VERY IMPORTANT)

### 1. Credentials

- Access Key ID
- Secret Access Key

---

### 2. Profiles

- Multiple configurations

---

### 3. Commands

Structure:
aws <service> <operation>

Example:
aws ec2 describe-instances

---

## 🧠 Architectural Logic (Why AWS CLI?)

### When to Use CLI:

✅ Automation scripts  
✅ DevOps workflows  
✅ Infrastructure management  
✅ Quick operations  

👉 CLI = Automation layer

---

## ⚖️ CLI vs SDK vs Console (VERY IMPORTANT)

| Tool | Use Case |
|-----|----------|
| CLI | Terminal automation |
| SDK | Application integration |
| Console | Manual UI |

👉 CLI = fastest for ops  
👉 SDK = for code  
👉 Console = for humans  

---

## ⚡ Performance & Scaling

- Direct API calls
- Can script bulk operations

---

## 💸 Cost Optimization

- No cost for CLI itself
- Helps automate cost-saving tasks

---

## 🔐 Security (VERY IMPORTANT)

### Best Practices:

- Use IAM roles (NOT root user)
- Rotate keys
- Use least privilege

---

## 🔄 Integration with Other Services

- Works with ALL AWS services:
  - [[Amazon EC2]]
  - [[Amazon S3]]
  - [[AWS Lambda]]
  - [[Amazon RDS]]

---

## 🚀 Real-World Architecture (Pro Level)

### ⚙️ Automation Script

1. CLI script:
   - Launch EC2
   - Configure S3
   - Deploy app

👉 Infrastructure automation

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. CLI = NOT a service  
👉 It’s a tool

🔥 2. Uses AWS APIs  
👉 Backend communication

🔥 3. Requires credentials  
👉 IAM-based

🔥 4. Key keyword:
> “Manage AWS using command line / automation”

👉 Answer = AWS CLI

---

## 🧠 Advanced Architect Insight

CLI is key for **Infrastructure as Code (IaC)** workflows:

CLI  
→ Scripts  
→ Automation  
→ Scalable ops  

👉 Foundation for DevOps

---

## 📊 When NOT to Use CLI

❌ GUI preference → Use Console  
❌ Application integration → Use SDK  

---

## 🔥 One-Line Summary

👉 AWS CLI = Tool to manage AWS services via command line

---

## 🔗 Related Services

- AWS SDK
- AWS CloudFormation
- AWS Systems Manager