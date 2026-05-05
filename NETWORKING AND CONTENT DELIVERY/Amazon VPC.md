# 🧠 Amazon VPC (Virtual Private Cloud)

## 🔗 Service Type
#Networking #Security #Core #Architecture

---

## 📌 What is Amazon VPC?

Amazon VPC is a **logically isolated virtual network** in AWS where you:

- Launch resources (EC2, RDS, etc.)
- Control networking (IP, routing, security)

👉 VPC = “Your private data center in AWS”

---

## ⚙️ How It Works (Architecture Thinking)

1. Create VPC:
   - CIDR block (e.g., 10.0.0.0/16)

2. Create subnets:
   - Public / Private

3. Attach gateways:
   - Internet Gateway (IGW)
   - NAT Gateway

4. Configure routing + security

👉 Network → Subnet → Routing → Security

---

## 🏗️ Core Components (VERY IMPORTANT)

### 1. CIDR Block

- Defines IP range

Example:
10.0.0.0/16

---

### 2. Subnets (CRITICAL)

#### Public Subnet
- Has route to IGW

#### Private Subnet
- No direct internet access

👉 Design for security

---

### 3. Internet Gateway (IGW)

- Enables internet access

---

### 4. NAT Gateway (VERY IMPORTANT)

- Allows private subnet → internet (OUTBOUND ONLY)

👉 Private resources stay hidden

---

### 5. Route Tables

- Define traffic flow

Example:
0.0.0.0/0 → IGW

---

### 6. Security Groups (CRITICAL)

- Stateful firewall

👉 Allow rules only

---

### 7. Network ACL (NACL)

- Stateless firewall

👉 Allow + Deny rules

---

## 🧠 Architectural Logic (VERY IMPORTANT)

### Public vs Private Design

- Public:
  - Load balancers
  - Bastion hosts

- Private:
  - App servers
  - Databases

👉 Separation = security

---

## ⚖️ Security Groups vs NACL (VERY IMPORTANT)

| Feature | Security Group | NACL |
|--------|--------------|------|
| Type | Stateful | Stateless |
| Rules | Allow only | Allow + Deny |
| Level | Instance | Subnet |

👉 SG = instance protection  
👉 NACL = subnet protection  

---

## ⚡ High Availability (CRITICAL)

- Use multiple AZs
- Subnets across AZs

👉 Fault tolerance

---

## ⚡ Connectivity Options (VERY IMPORTANT)

### 1. Internet Access
- IGW + public subnet

---

### 2. Private Internet Access
- NAT Gateway

---

### 3. Hybrid Connectivity

- [[AWS Site-to-Site VPN]]
- [[AWS Direct Connect]]

---

### 4. VPC Peering

- Connect VPCs

---

### 5. AWS Transit Gateway

- Hub-and-spoke networking

---

## 💸 Cost Optimization

- NAT Gateway costs money ⚠️
- Use VPC endpoints when possible

---

## 🔐 Security (VERY IMPORTANT)

- Security Groups
- NACLs
- Private subnets
- No public IPs for sensitive resources

---

## 🔄 Integration with Other Services

- [[Amazon EC2]] → compute
- [[Amazon RDS]] → database
- [[Elastic Load Balancing]] → traffic distribution
- [[AWS Lambda]] → VPC-enabled functions

---

## 🚀 Real-World Architecture (Pro Level)

### 🌐 Highly Available Web App

Public Subnet:
- ALB

Private Subnet:
- EC2 app servers
- RDS database

Routing:
- IGW (public)
- NAT Gateway (private)

👉 Secure + scalable architecture

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Private subnet ≠ no internet  
👉 NAT allows outbound

🔥 2. Security Groups are stateful  
👉 Return traffic allowed

🔥 3. NACL is stateless  
👉 Must allow both directions

🔥 4. NAT Gateway is AZ-specific  
👉 Use one per AZ for HA

🔥 5. Key keyword:
> “Design secure network / isolate resources / VPC architecture”

👉 Answer = VPC concepts

---

## 🧠 Advanced Architect Insight

Best practice architecture:

Public subnet:
- Load balancer

Private subnet:
- App + DB

Multi-AZ:
- High availability

👉 Production-ready design

---

## 📊 When NOT to Use Certain Features

❌ Public DB → BAD practice  
❌ Single AZ → NOT highly available  
❌ No NAT → no outbound internet  

---

## 🔥 One-Line Summary

👉 Amazon VPC = Your isolated, customizable network in AWS

---

## 🔗 Related Services

- AWS Direct Connect
- AWS Site-to-Site VPN
- AWS Client VPN
- Elastic Load Balancing