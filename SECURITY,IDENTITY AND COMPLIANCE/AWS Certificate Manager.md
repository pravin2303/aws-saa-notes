# 🧠 AWS Certificate Manager (ACM)

## 🔗 Service Type
#Security #Encryption #SSL #Certificates

---

## 📌 What is AWS Certificate Manager?

AWS Certificate Manager (ACM) is a service that:

- Provides SSL/TLS certificates
- Enables HTTPS for applications
- Automatically manages certificate lifecycle

👉 ACM = “Manage SSL certificates easily”

---

## ⚙️ How It Works (Architecture Thinking)

1. Request certificate:
   - Public or private

2. Validate domain:
   - DNS validation (Route 53)
   - Email validation

3. Attach certificate to:
   - [[Elastic Load Balancing]]
   - [[Amazon CloudFront]]
   - API Gateway

4. ACM handles renewal automatically

👉 Request → Validate → Attach → Auto-renew

---

## 🏗️ Core Concepts (VERY IMPORTANT)

### 1. Public Certificates

- For internet-facing apps
- FREE (important!)

---

### 2. Private Certificates

- For internal apps (via ACM PCA)

---

### 3. Domain Validation (CRITICAL)

- DNS validation (MOST COMMON)
- Email validation

---

### 4. Auto Renewal (IMPORTANT)

- No manual renewal required

---

## 🧠 Architectural Logic (VERY IMPORTANT)

### When to Use ACM:

✅ HTTPS for web apps  
✅ Secure communication  
✅ Avoid manual certificate management  
✅ Integrate with AWS services  

👉 ACM = Secure application layer

---

## ⚖️ ACM vs Self-Managed Certificates (VERY IMPORTANT)

| Feature | ACM | Self-managed |
|--------|-----|-------------|
| Renewal | Automatic | Manual |
| Cost | Free (public certs) | Paid |
| Management | Easy | Complex |

👉 ACM = best choice in AWS  

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Free Public Certificates
- No extra cost

---

### 2. Automatic Renewal
- Fully managed

---

### 3. Easy Integration
- Works with ELB, CloudFront

---

### 4. Secure Storage
- Keys managed by AWS

---

## ⚡ Performance & Scaling

- No performance overhead
- Fully managed

---

## 💸 Cost Optimization

- Public certs = FREE
- Private certs = paid

---

## 🔐 Security (VERY IMPORTANT)

- Enables HTTPS (TLS encryption)
- Protects data in transit

---

## 🔄 Integration with Other Services

- [[Elastic Load Balancing]] → HTTPS termination
- [[Amazon CloudFront]] → CDN security
- [[Amazon Route 53]] → DNS validation
- API Gateway → secure APIs

---

## 🚀 Real-World Architecture (Pro Level)

### 🔐 Secure Web Application

User → HTTPS  
→ CloudFront / ALB  
→ ACM certificate  
→ Backend  

👉 Secure communication

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. ACM certs are FREE (public)  
👉 Important detail

🔥 2. Cannot export private key (for public certs)  
👉 Key limitation

🔥 3. Used only with supported AWS services  
👉 Not for direct EC2 (without ALB)

🔥 4. DNS validation = preferred  
👉 Faster + automated

🔥 5. Key keyword:
> “SSL / HTTPS / certificate / encryption in transit”

👉 Answer = ACM

---

## 🧠 Advanced Architect Insight

ACM enables **secure-by-default architecture**:

User  
→ HTTPS  
→ AWS service  
→ Backend  

👉 Encrypted communication

---

## 📊 When NOT to Use ACM

❌ Need external/private key control → Use IAM certificates  
❌ Non-AWS services → use external CA  

---

## 🔥 One-Line Summary

👉 AWS ACM = Managed service for SSL/TLS certificates with automatic renewal

---

## 🔗 Related Services

- Amazon CloudFront
- Elastic Load Balancing
- Amazon Route 53
- AWS WAF