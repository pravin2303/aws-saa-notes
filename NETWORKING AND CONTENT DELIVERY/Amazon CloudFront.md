# 🧠 Amazon CloudFront

## 🔗 Service Type
#Networking #CDN #Performance #Security

---

## 📌 What is Amazon CloudFront?

Amazon CloudFront is a **Content Delivery Network (CDN)** that:

- Delivers content globally with low latency
- Caches content at edge locations

👉 CloudFront = “Serve content closer to users”

---

## ⚙️ How It Works (Architecture Thinking)

1. User requests content

2. CloudFront checks edge location cache

3. If NOT cached:
   - Fetch from origin:
     - [[Amazon S3]]
     - [[Amazon EC2]]
     - ALB

4. Cache and deliver to user

👉 User → Edge → Origin

---

## 🏗️ Core Components (VERY IMPORTANT)

### 1. Edge Locations

- Global cache servers

---

### 2. Origin

- Source of content:
  - S3
  - EC2
  - ALB

---

### 3. Distribution

- Configuration of CDN

---

### 4. Cache Behavior (CRITICAL)

- Rules for caching:
  - TTL
  - Path patterns

---

## 🧠 Architectural Logic (Why CloudFront?)

### When to Choose CloudFront:

✅ Reduce latency  
✅ Improve performance  
✅ Secure content delivery  
✅ Global applications  

👉 CloudFront = Performance + security layer

---

## ⚖️ CloudFront vs S3 Direct Access (VERY IMPORTANT)

| Feature | CloudFront | S3 |
|--------|------------|----|
| Performance | Global CDN | Single region |
| Security | Advanced | Basic |
| Latency | Low | Higher |

👉 Use CloudFront in front of S3

---

## ⚖️ CloudFront vs API Gateway

| Feature | CloudFront | API Gateway |
|--------|------------|-------------|
| Use case | Content delivery | API management |
| Caching | Yes | Limited |

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Caching (CRITICAL)
- Reduces origin load

---

### 2. Low Latency
- Global edge network

---

### 3. DDoS Protection
- Integrated with AWS Shield

---

### 4. HTTPS Support
- SSL/TLS encryption

---

### 5. Signed URLs & Cookies
- Secure content access

---

## ⚡ Performance & Scaling

- Global scale
- Handles high traffic

---

## 💸 Cost Optimization

- Reduces origin costs
- Pay for:
  - Data transfer
  - Requests

---

## 🔐 Security (VERY IMPORTANT)

- AWS Shield (DDoS protection)
- AWS WAF integration
- HTTPS encryption

---

## 🔄 Integration with Other Services

- [[Amazon S3]] → static content
- [[Elastic Load Balancing]] → dynamic apps
- [[AWS WAF]] → security
- [[AWS Shield]] → DDoS protection

---

## 🚀 Real-World Architecture (Pro Level)

### 🌍 Global Web Application

User → CloudFront  
→ ALB  
→ EC2  

Static content → S3 via CloudFront  

👉 High-performance architecture

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. CloudFront = CDN  
👉 Not storage

🔥 2. Caching reduces latency  
👉 Key benefit

🔥 3. Works with S3 + ALB  
👉 Important integration

🔥 4. Key keyword:
> “Low latency / global delivery / caching / CDN”

👉 Answer = CloudFront

---

## 🧠 Advanced Architect Insight

CloudFront enables **edge-optimized architecture**:

User  
→ Edge cache  
→ Origin  

👉 Faster + scalable systems

---

## 📊 When NOT to Use CloudFront

❌ Internal apps → Use ALB  
❌ Storage → Use [[Amazon S3]]  

---

## 🔥 One-Line Summary

👉 CloudFront = Global CDN to deliver content with low latency and high performance

---

## 🔗 Related Services

- Amazon S3
- AWS WAF
- AWS Shield
- Elastic Load Balancing