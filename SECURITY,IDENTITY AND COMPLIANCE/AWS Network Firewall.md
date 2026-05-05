# 🧠 AWS Network Firewall

## 🔗 Service Type
#Security #Networking #Firewall #Inspection

---

## 📌 What is AWS Network Firewall?

AWS Network Firewall is a service that:

- Protects your VPC at the network layer
- Filters and inspects traffic (inbound/outbound)

👉 Network Firewall = “Advanced firewall inside your VPC”

---

## ⚙️ How It Works (Architecture Thinking)

1. Deploy firewall in dedicated subnet

2. Route traffic through firewall

3. Firewall inspects:
   - IP
   - Port
   - Protocol
   - Content (deep inspection)

4. Allow / Deny traffic

👉 Traffic → Firewall → Filter → Destination

---

## 🏗️ Core Concepts (VERY IMPORTANT)

### 1. Firewall Endpoint (CRITICAL)

- Deployed in subnet
- Processes traffic

---

### 2. Rule Groups

Types:
- Stateless rules
- Stateful rules (IMPORTANT)

---

### 3. Policies

- Define how rules are applied

---

## 🧠 Architectural Logic (VERY IMPORTANT)

### When to Use Network Firewall:

✅ Control VPC traffic  
✅ Deep packet inspection  
✅ Centralized security policy  
✅ Compliance requirements  

👉 Network Firewall = network-level protection

---

## ⚖️ Network Firewall vs Security Groups vs NACL (VERY IMPORTANT)

| Feature | Network Firewall | Security Group | NACL |
|--------|----------------|---------------|------|
| Level | VPC-wide | Instance | Subnet |
| Type | Stateful + DPI | Stateful | Stateless |
| Complexity | Advanced | Simple | Basic |

👉 Firewall = advanced control  

---

## ⚖️ Network Firewall vs AWS WAF

| Feature | Network Firewall | WAF |
|--------|------------------|-----|
| Layer | Network (L3–L4 + DPI) | Application (L7) |
| Use case | VPC traffic | HTTP filtering |

👉 Firewall = network  
👉 WAF = web  

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Stateful Inspection (CRITICAL)
- Tracks connections

---

### 2. Stateless Filtering
- Fast filtering rules

---

### 3. Deep Packet Inspection
- Analyze traffic content

---

### 4. Centralized Security
- Apply rules across VPC

---

## ⚡ Performance & Scaling

- Automatically scales
- High throughput

---

## 💸 Cost Optimization

- Pay for:
  - Endpoints
  - Traffic processed

---

## 🔐 Security (VERY IMPORTANT)

- Strong network protection
- Prevent unauthorized access

---

## 🔄 Integration with Other Services

- [[Amazon VPC]] → deployment
- [[AWS Transit Gateway]] → centralized inspection
- [[Amazon CloudWatch]] → monitoring

---

## 🚀 Real-World Architecture (Pro Level)

### 🛡️ Centralized Security VPC

All traffic  
→ Network Firewall  
→ Application VPC  

👉 Central inspection layer

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Network Firewall = VPC-level  
👉 Not instance-level

🔥 2. Supports deep packet inspection  
👉 Key feature

🔥 3. Requires routing through firewall  
👉 Important detail

🔥 4. Key keyword:
> “Inspect VPC traffic / centralized firewall / deep inspection”

👉 Answer = AWS Network Firewall

---

## 🧠 Advanced Architect Insight

Network Firewall enables **zero-trust network architecture**:

Traffic  
→ Inspected  
→ Allowed/Denied  

👉 Full control

---

## 📊 When NOT to Use Network Firewall

❌ Simple rules → Use Security Groups  
❌ Web filtering → Use [[AWS WAF]]  

---

## 🔥 One-Line Summary

👉 AWS Network Firewall = Advanced firewall to inspect and control VPC traffic

---

## 🔗 Related Services

- Amazon VPC
- AWS WAF
- AWS Transit Gateway
- Amazon CloudWatch