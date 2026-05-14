# 🧠 AWS Transit Gateway (TGW)

## 🔗 Service Type
#Networking #Connectivity #HubAndSpoke #Hybrid

---

## 📌 What is AWS Transit Gateway?

AWS Transit Gateway is a service that:

- Connects multiple VPCs and on-prem networks
- Acts as a central hub

👉 Transit Gateway = “Network hub for AWS”

---

## ⚙️ How It Works (Architecture Thinking)

1. Create Transit Gateway

2. Attach:
   - VPCs
   - VPN connections
   - Direct Connect

3. Configure routing

👉 Hub → Multiple networks

---

## 🏗️ Core Components (VERY IMPORTANT)

### 1. Attachments

- Connect resources to TGW:
  - VPC attachment
  - VPN attachment
  - Direct Connect attachment

---

### 2. Route Tables (CRITICAL)

- Control traffic flow between attachments

---

### 3. Hub-and-Spoke Model

- TGW = hub  
- VPCs = spokes  

---

## 🧠 Architectural Logic (VERY IMPORTANT)

### Without Transit Gateway:

- VPC Peering (complex mesh)

👉 n(n-1)/2 connections

---

### With Transit Gateway:

- Central hub

👉 Simplified architecture

---

## ⚖️ Transit Gateway vs VPC Peering (VERY IMPORTANT)

| Feature | Transit Gateway | VPC Peering |
|--------|----------------|-------------|
| Scale | High | Limited |
| Architecture | Hub-and-spoke | Mesh |
| Management | Easy | Complex |

👉 TGW = scalable  
👉 Peering = simple use case  

---

## ⚖️ Transit Gateway vs Direct Connect

| Feature | Transit Gateway | Direct Connect |
|--------|----------------|----------------|
| Purpose | Connect VPCs | Connect on-prem |
| Scope | AWS internal | Hybrid |

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Centralized Connectivity
- One hub for all networks

---

### 2. Scalable Architecture
- Supports many VPCs

---

### 3. Hybrid Connectivity (IMPORTANT)
- Works with:
  - VPN
  - Direct Connect

---

### 4. Route Isolation
- Separate route tables

---

## ⚡ Performance & Scaling

- High throughput
- Automatically scales

---

## 💸 Cost Optimization

- Reduces complexity
- Fewer connections than peering

---

## 🔐 Security

- Route table isolation
- Controlled traffic flow

---

## 🔄 Integration with Other Services

- [[Amazon VPC]] → network attachments
- [[AWS Site-to-Site VPN]] → hybrid connectivity
- [[AWS Direct Connect]] → private connection

---

## 🚀 Real-World Architecture (Pro Level)

### 🏢 Multi-VPC Enterprise Network

Multiple VPCs  
→ Transit Gateway (hub)  
→ On-prem via VPN/DX  

👉 Centralized network

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. TGW = hub-and-spoke ONLY  
👉 Not mesh

🔥 2. Replaces complex VPC peering  
👉 Key concept

🔥 3. Uses route tables for control  
👉 Important detail

🔥 4. Key keyword:
> “Connect multiple VPCs / centralized networking / hub-and-spoke”

👉 Answer = Transit Gateway

---

## 🧠 Advanced Architect Insight

Transit Gateway enables **enterprise-grade networking**:

VPCs  
→ TGW  
→ Central routing  

👉 Scalable + manageable

---

## 📊 When NOT to Use Transit Gateway

❌ Small setup (2 VPCs) → Use peering  
❌ Single VPC → unnecessary  

---

## 🔥 One-Line Summary

👉 AWS Transit Gateway = Central hub to connect multiple VPCs and networks

---

## 🔗 Related Services

- Amazon VPC
- AWS Direct Connect
- AWS Site-to-Site VPN
- VPC Peering