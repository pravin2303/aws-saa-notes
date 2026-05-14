# 🧠 AWS Shield

## 🔗 Service Type
#Security #DDoS #Protection #Networking

---

## 📌 What is AWS Shield?

AWS Shield is a service that:

- Protects applications from Distributed Denial of Service (DDoS) attacks
- Automatically detects and mitigates attacks

👉 Shield = “DDoS protection for AWS resources”

---

## ⚙️ How It Works (Architecture Thinking)

1. Traffic flows into AWS services:
   - [[Amazon CloudFront]]
   - [[Elastic Load Balancing]]
   - [[Amazon Route 53]]

2. Shield monitors traffic patterns

3. Detects abnormal spikes (attack)

4. Automatically mitigates attack

👉 Traffic → Detection → Mitigation

---

## 🏗️ Types of AWS Shield (VERY IMPORTANT)

### 1. Shield Standard (FREE)

- Enabled by default
- Protects against:
  - Layer 3 & Layer 4 attacks

---

### 2. Shield Advanced (PAID)

- Enhanced protection
- Covers:
  - Layer 7 (application attacks)
- Includes:
  - DDoS response team (DRT)
  - Cost protection

---

## 🧠 Architectural Logic (VERY IMPORTANT)

### When to Use Shield:

✅ Protect public applications  
✅ Prevent DDoS attacks  
✅ Secure web services  
✅ Ensure availability  

👉 Shield = availability protection

---

## ⚖️ Shield vs AWS WAF (VERY IMPORTANT)

| Feature | Shield | WAF |
|--------|--------|-----|
| Protection | DDoS | Application layer |
| Focus | Network attacks | HTTP filtering |

👉 Shield = attack mitigation  
👉 WAF = request filtering  

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Automatic Protection
- No setup needed (Standard)

---

### 2. Real-Time Detection
- Identifies attacks quickly

---

### 3. Advanced Protection (Shield Advanced)
- Application-level protection

---

### 4. Integration with AWS Services
- CloudFront, ALB, Route 53

---

## ⚡ Performance & Scaling

- Global protection
- Scales automatically

---

## 💸 Cost Optimization

- Shield Standard = FREE  
- Shield Advanced = paid

---

## 🔐 Security (VERY IMPORTANT)

- Protects availability
- Works with WAF for layered security

---

## 🔄 Integration with Other Services

- [[Amazon CloudFront]] → edge protection
- [[Elastic Load Balancing]] → traffic protection
- [[Amazon Route 53]] → DNS protection
- [[AWS WAF]] → application filtering

---

## 🚀 Real-World Architecture (Pro Level)

### 🛡️ Secure Web Application

User  
→ CloudFront (Shield)  
→ WAF  
→ ALB  
→ EC2  

👉 Multi-layer protection

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Shield Standard = automatic + free  
👉 Always enabled

🔥 2. Shield Advanced = paid  
👉 Includes Layer 7 protection

🔥 3. Works with CloudFront, ALB, Route 53  
👉 Key integration

🔥 4. Key keyword:
> “DDoS protection / protect against attacks / availability”

👉 Answer = AWS Shield

---

## 🧠 Advanced Architect Insight

Best practice:

Shield + WAF  

👉 Combines:
- DDoS protection (Shield)
- Request filtering (WAF)

---

## 📊 When NOT to Use Shield

❌ Block specific IPs → Use [[AWS WAF]]  
❌ Authentication → Use IAM/Cognito  

---

## 🔥 One-Line Summary

👉 AWS Shield = Managed DDoS protection service for AWS applications

---

## 🔗 Related Services

- AWS WAF
- Amazon CloudFront
- Amazon Route 53
- Elastic Load Balancing