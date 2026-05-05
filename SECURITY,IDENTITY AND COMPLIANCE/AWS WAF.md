# 🧠 AWS WAF (Web Application Firewall)

## 🔗 Service Type
#Security #WebProtection #Filtering #Layer7

---

## 📌 What is AWS WAF?

AWS WAF is a service that:

- Protects web applications from common web exploits
- Filters HTTP/HTTPS requests

👉 WAF = “Application-layer protection”

---

## ⚙️ How It Works (Architecture Thinking)

1. User sends HTTP request

2. WAF inspects request:
   - Headers
   - Body
   - IP

3. Applies rules:
   - Allow / Block / Count

4. Forward request if allowed

👉 Request → Inspect → Filter → Forward

---

## 🏗️ Core Concepts (VERY IMPORTANT)

### 1. Web ACL (CRITICAL)

- Collection of rules

---

### 2. Rules

Types:
- IP-based
- Geo-based
- Rate-based (IMPORTANT)
- Pattern matching

---

### 3. Rule Groups

- Managed or custom rules

---

## 🧠 Architectural Logic (VERY IMPORTANT)

### When to Use WAF:

✅ Protect web apps  
✅ Block malicious traffic  
✅ Prevent:
- SQL injection
- Cross-site scripting (XSS)  
✅ Control traffic patterns  

👉 WAF = request filtering

---

## ⚖️ WAF vs Shield (VERY IMPORTANT)

| Feature | WAF | Shield |
|--------|-----|--------|
| Layer | 7 (HTTP) | 3/4 (network) |
| Purpose | Filter requests | DDoS protection |

👉 WAF = app security  
👉 Shield = network protection  

---

## ⚖️ WAF vs Security Groups

| Feature | WAF | Security Group |
|--------|-----|---------------|
| Layer | Application | Network |
| Rules | HTTP-based | Port-based |

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. SQL Injection Protection
- Detect malicious queries

---

### 2. XSS Protection
- Prevent script attacks

---

### 3. Rate Limiting (CRITICAL)
- Block excessive requests

---

### 4. Managed Rule Sets
- AWS-provided security rules

---

## ⚡ Performance & Scaling

- Global (with CloudFront)
- Automatically scales

---

## 💸 Cost Optimization

- Pay per:
  - Rules
  - Requests

---

## 🔐 Security (VERY IMPORTANT)

- Layer 7 protection
- Works with Shield

---

## 🔄 Integration with Other Services

- [[Amazon CloudFront]] → global protection
- [[Elastic Load Balancing]] → app protection
- [[Amazon API Gateway]] → API security
- [[AWS Shield]] → DDoS protection

---

## 🚀 Real-World Architecture (Pro Level)

### 🛡️ Secure Web Application

User  
→ CloudFront  
→ WAF  
→ ALB  
→ EC2  

👉 Multi-layer security

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. WAF = Layer 7 ONLY  
👉 HTTP/HTTPS

🔥 2. Protects against SQL injection, XSS  
👉 Key feature

🔥 3. Uses Web ACL  
👉 Important concept

🔥 4. Works with CloudFront, ALB, API Gateway  
👉 Integration

🔥 5. Key keyword:
> “Block malicious HTTP requests / SQL injection / XSS”

👉 Answer = AWS WAF

---

## 🧠 Advanced Architect Insight

Best practice:

WAF + Shield + CloudFront  

👉 Full protection stack

---

## 📊 When NOT to Use WAF

❌ DDoS protection → Use [[AWS Shield]]  
❌ Network-level filtering → Use Security Groups  

---

## 🔥 One-Line Summary

👉 AWS WAF = Protects web apps by filtering HTTP/HTTPS traffic

---

## 🔗 Related Services

- AWS Shield
- Amazon CloudFront
- Elastic Load Balancing
- Amazon API Gateway