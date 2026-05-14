# 🧠 AWS Site-to-Site VPN

## 🔗 Service Type
#Networking #HybridCloud #VPN #Security

---

## 📌 What is AWS Site-to-Site VPN?

AWS Site-to-Site VPN is a service that:

- Connects your on-premises network to AWS VPC
- Over the public internet using encrypted tunnels

👉 Site-to-Site VPN = “Secure network-to-network connection”

---

## ⚙️ How It Works (Architecture Thinking)

1. On-premises data center has VPN device

2. AWS creates Virtual Private Gateway (VGW)

3. Two encrypted tunnels are established

4. Traffic flows securely

👉 Data center → VPN → AWS VPC

---

## 🏗️ Core Components (VERY IMPORTANT)

### 1. Customer Gateway (CGW)

- Your on-prem VPN device

---

### 2. Virtual Private Gateway (VGW)

- AWS side VPN endpoint

---

### 3. VPN Connection

- Secure connection between CGW and VGW

---

### 4. Tunnels (CRITICAL)

- Two tunnels for redundancy

---

## 🧠 Architectural Logic (VERY IMPORTANT)

### When to Choose Site-to-Site VPN:

✅ Hybrid architecture  
✅ Secure connection over internet  
✅ Quick setup  
✅ Backup for Direct Connect  

👉 Site-to-Site VPN = Hybrid connectivity

---

## ⚖️ Site-to-Site VPN vs Direct Connect (VERY IMPORTANT)

| Feature | Site-to-Site VPN | Direct Connect |
|--------|-----------------|----------------|
| Network | Internet | Dedicated line |
| Setup | Fast | Slow |
| Cost | Low | High |
| Performance | Variable | Consistent |

👉 VPN = quick & flexible  
👉 Direct Connect = stable & high performance  

---

## ⚖️ Site-to-Site VPN vs Client VPN

| Feature | Site-to-Site VPN | Client VPN |
|--------|-----------------|-----------|
| Users | Networks | Individuals |
| Use case | Data center | Remote users |

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Encrypted Tunnels
- Secure communication

---

### 2. High Availability (CRITICAL)
- Two tunnels automatically

---

### 3. Dynamic Routing (BGP)
- Automatic route updates

---

### 4. Hybrid Connectivity
- Connect on-prem to AWS

---

## ⚡ Performance & Scaling

- Limited by internet bandwidth
- Scales with network

---

## 💸 Cost Optimization

- Low cost setup
- No physical infrastructure

---

## 🔐 Security (VERY IMPORTANT)

- IPsec encryption
- Secure tunnels

---

## 🔄 Integration with Other Services

- [[Amazon VPC]] → target network
- [[AWS Direct Connect]] → hybrid architecture
- [[AWS Transit Gateway]] → multi-VPC connectivity

---

## 🚀 Real-World Architecture (Pro Level)

### 🏢 Hybrid Network Setup

Data center  
→ Site-to-Site VPN  
→ VPC  
→ AWS services  

Backup:
→ Direct Connect (optional)

👉 Hybrid cloud architecture

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Uses public internet  
👉 But encrypted

🔥 2. Two tunnels always  
👉 High availability

🔥 3. Performance depends on internet  
👉 Not guaranteed

🔥 4. Key keyword:
> “Connect data center to AWS securely over internet”

👉 Answer = Site-to-Site VPN

---

## 🧠 Advanced Architect Insight

Best practice:

Direct Connect + VPN  

👉 Combines:
- Reliability (DX)
- Backup (VPN)

---

## 📊 When NOT to Use Site-to-Site VPN

❌ High-performance needs → Use [[AWS Direct Connect]]  
❌ Remote users → Use [[AWS Client VPN]]  

---

## 🔥 One-Line Summary

👉 AWS Site-to-Site VPN = Secure connection between on-prem networks and AWS over the internet

---

## 🔗 Related Services

- Amazon VPC
- AWS Direct Connect
- AWS Transit Gateway
- AWS Client VPN