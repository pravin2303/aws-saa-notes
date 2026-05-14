## AWS Systems Manager – CLF-C02 Scope 🛠️📊

**AWS Systems Manager** is a service that helps you **manage and operate your AWS resources** at scale.

It is mainly used to manage:

- EC2 instances
    
- On-premises servers
    
- Hybrid environments
    

---

## What Systems Manager Does

✔ Manage instances remotely  
✔ Automate operational tasks  
✔ Apply patches  
✔ Store configuration parameters securely

---

## Key Features (High-Level for CLF-C02)

### 1️⃣ Session Manager

Securely connect to EC2 instances **without SSH keys**.

### 2️⃣ Patch Manager

Automate OS patching.

### 3️⃣ Parameter Store

Store configuration data and secrets securely.

---

## Why It Is Important

✔ Improves security  
✔ Reduces operational overhead  
✔ Centralized management  
✔ No need to open SSH ports (using Session Manager)

---

## Example (Exam Scenario)

If question says:

“Company wants to patch EC2 instances automatically.”

Correct answer → AWS Systems Manager.

If question says:

“Securely connect to EC2 without SSH.”

Correct answer → Session Manager (part of Systems Manager).

---

## Systems Manager vs CloudWatch (Exam Concept)

|Service|Purpose|
|---|---|
|CloudWatch|Monitor metrics|
|Systems Manager|Manage & operate instances|

---

## Key Exam Keywords 🎯

- “Remote instance management” → Systems Manager
    
- “Patch EC2 automatically” → Systems Manager
    
- “Store configuration parameters” → Parameter Store
    

---

### For CLF-C02 remember:

> Systems Manager = Manage, patch, and operate AWS resources