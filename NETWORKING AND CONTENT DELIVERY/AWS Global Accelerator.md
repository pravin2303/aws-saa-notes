# 🧠 AWS Global Accelerator

## 🔗 Service Type
#Networking #Performance #Global #TrafficRouting

---

## 📌 What is AWS Global Accelerator?

AWS Global Accelerator is a service that:

- Improves availability and performance of applications
- Routes traffic through AWS global network

👉 Global Accelerator = “Fast, intelligent global traffic routing”

---

## ⚙️ How It Works (Architecture Thinking)

1. User connects to static IP (Global Accelerator)

2. Traffic enters AWS edge location

3. Routed via AWS global backbone

4. Sent to optimal endpoint:
   - [[Elastic Load Balancing]]
   - [[Amazon EC2]]
   - IP address

👉 User → Edge → AWS network → Endpoint

---

## 🏗️ Core Components (VERY IMPORTANT)

### 1. Accelerator

- Provides static IPs

---

### 2. Listener

- Defines protocol (TCP/UDP)

---

### 3. Endpoint Groups

- Group of endpoints per region

---

### 4. Endpoints (CRITICAL)

- ALB, NLB, EC2, Elastic IP

---

## 🧠 Architectural Logic (VERY IMPORTANT)

### When to Choose Global Accelerator:

✅ Improve global app performance  
✅ Reduce latency  
✅ Use static IP for apps  
✅ Need fast failover  

👉 Global Accelerator = network optimization

---

## ⚖️ Global Accelerator vs CloudFront (VERY IMPORTANT)

| Feature | Global Accelerator | CloudFront |
|--------|------------------|------------|
| Use case | Dynamic apps | Static content |
| Protocol | TCP/UDP | HTTP/HTTPS |
| Caching | No | Yes |

👉 CloudFront = CDN  
👉 Global Accelerator = network routing  

---

## ⚖️ Global Accelerator vs Route 53

| Feature | Global Accelerator | Route 53 |
|--------|------------------|----------|
| Routing | Network layer | DNS layer |
| Failover | Fast (milliseconds) | Slower (DNS TTL) |

👉 Global Accelerator = faster failover  

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Static IP Addresses (CRITICAL)
- Fixed entry point

---

### 2. AWS Global Network
- Low latency routing

---

### 3. Fast Failover
- Automatic endpoint switching

---

### 4. Health Checks
- Detect unhealthy endpoints

---

## ⚡ Performance & Scaling

- Ultra-low latency
- Global reach

---

## 💸 Cost Optimization

- Pay for:
  - Accelerator usage
  - Data transfer

---

## 🔐 Security

- DDoS protection via AWS Shield
- Traffic stays in AWS network

---

## 🔄 Integration with Other Services

- [[Elastic Load Balancing]] → backend endpoints
- [[Amazon EC2]] → compute
- [[Amazon Route 53]] → DNS
- [[Amazon CloudFront]] → CDN (optional combo)

---

## 🚀 Real-World Architecture (Pro Level)

### 🌍 Global Low-Latency Application

User  
→ Global Accelerator (static IP)  
→ AWS edge  
→ ALB (closest region)  
→ EC2  

👉 Fast + reliable system

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. No caching  
👉 Not CDN

🔥 2. Uses TCP/UDP  
👉 Not HTTP-focused

🔥 3. Static IPs provided  
👉 Important feature

🔥 4. Faster than Route 53 failover  
👉 Key differentiator

🔥 5. Key keyword:
> “Improve global performance / static IP / fast failover”

👉 Answer = Global Accelerator

---

## 🧠 Advanced Architect Insight

Global Accelerator enables **network-level optimization**:

User  
→ AWS backbone  
→ Best endpoint  

👉 Faster + more reliable than internet routing

---

## 📊 When NOT to Use Global Accelerator

❌ Static content → Use [[Amazon CloudFront]]  
❌ DNS-only routing → Use [[Amazon Route 53]]  

---

## 🔥 One-Line Summary

👉 AWS Global Accelerator = Improves global application performance using AWS network

---

## 🔗 Related Services

- Amazon CloudFront
- Amazon Route 53
- Elastic Load Balancing
- Amazon EC2