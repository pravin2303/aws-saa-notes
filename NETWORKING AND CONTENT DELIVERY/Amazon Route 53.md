# 🧠 Amazon Route 53

## 🔗 Service Type
#Networking #DNS #Routing #HighAvailability

---

## 📌 What is Amazon Route 53?

Amazon Route 53 is a **scalable DNS service** that:

- Translates domain names → IP addresses
- Routes traffic to AWS resources

👉 Route 53 = “DNS + intelligent traffic routing”

---

## ⚙️ How It Works (Architecture Thinking)

1. User enters domain (example.com)

2. Route 53 resolves:
   - Domain → IP

3. Routes to:
   - [[Amazon CloudFront]]
   - [[Elastic Load Balancing]]
   - [[Amazon S3]]
   - EC2

👉 Domain → DNS → Resource

---

## 🏗️ Core Concepts (VERY IMPORTANT)

### 1. Hosted Zone

- Container for domain records

---

### 2. DNS Records

- A → IP address  
- CNAME → domain alias  
- Alias → AWS resource (IMPORTANT)

---

### 3. TTL (Time To Live)

- Cache duration

---

## 🧠 Architectural Logic (VERY IMPORTANT)

Route 53 is not just DNS — it’s **traffic routing engine**

👉 It decides:
- WHERE traffic goes
- HOW traffic is distributed

---

## ⚖️ Routing Policies (VERY IMPORTANT — HIGHLY TESTED)

### 1. Simple Routing

- Single resource

---

### 2. Weighted Routing

- Split traffic (e.g., 70% / 30%)

👉 Use for:
- Blue/Green deployment

---

### 3. Latency-Based Routing

- Route to nearest region

👉 Low latency

---

### 4. Failover Routing (CRITICAL)

- Primary → Secondary

👉 High availability

---

### 5. Geolocation Routing

- Based on user location

---

### 6. Multi-Value Routing

- Return multiple healthy IPs

---

## ⚡ Health Checks (CRITICAL)

- Monitor endpoints
- Automatically reroute traffic

👉 Enables failover

---

## ⚡ High Availability

- Global service
- Built-in redundancy

---

## 💸 Cost Optimization

- Pay per:
  - Hosted zones
  - Queries

---

## 🔐 Security

- DNS-level protection
- Works with:
  - [[AWS Shield]]
  - [[AWS WAF]]

---

## 🔄 Integration with Other Services

- [[Amazon CloudFront]] → CDN
- [[Elastic Load Balancing]] → traffic distribution
- [[Amazon S3]] → static hosting
- [[Amazon EC2]] → compute

---

## 🚀 Real-World Architecture (Pro Level)

### 🌍 Multi-Region Failover

User → Route 53  
→ Primary region (ALB)  

If failure:
→ Secondary region  

👉 High availability architecture

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Route 53 = DNS service  
👉 NOT load balancer

🔥 2. Alias record = AWS resource  
👉 No cost + better performance

🔥 3. Failover requires health checks  
👉 Important detail

🔥 4. Latency routing = closest region  
👉 NOT lowest load

🔥 5. Key keyword:
> “DNS / domain routing / failover / latency-based routing”

👉 Answer = Route 53

---

## 🧠 Advanced Architect Insight

Route 53 enables **global traffic control**:

User  
→ Route 53  
→ Best endpoint  

👉 Intelligent routing layer

---

## 📊 When NOT to Use Route 53

❌ Load balancing logic → Use [[Elastic Load Balancing]]  
❌ Content delivery → Use [[Amazon CloudFront]]  

---

## 🔥 One-Line Summary

👉 Route 53 = DNS service with intelligent routing policies

---

## 🔗 Related Services

- Amazon CloudFront
- Elastic Load Balancing
- AWS WAF
- AWS Shield