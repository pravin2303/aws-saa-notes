# 🧠 Elastic Load Balancing (ELB)

## 🔗 Service Type
#Networking #TrafficManagement #HighAvailability #Scaling

---

## 📌 What is Elastic Load Balancing?

Elastic Load Balancing automatically:

- Distributes incoming traffic across multiple targets
- Ensures high availability and fault tolerance

👉 ELB = “Distribute traffic efficiently”

---

## ⚙️ How It Works (Architecture Thinking)

1. User sends request

2. ELB receives traffic

3. Routes request to:
   - EC2 instances
   - Containers
   - IP targets

4. Performs health checks

👉 User → ELB → Targets

---

## 🏗️ Types of Load Balancers (VERY IMPORTANT — HIGHLY TESTED)

### 1. Application Load Balancer (ALB) — MOST IMPORTANT

- Layer 7 (HTTP/HTTPS)
- Smart routing:
  - Path-based
  - Host-based

👉 Use case:
- Web applications
- Microservices

---

### 2. Network Load Balancer (NLB)

- Layer 4 (TCP/UDP)
- Ultra-high performance
- Static IP

👉 Use case:
- High throughput
- Low latency apps

---

### 3. Gateway Load Balancer (GLB)

- Used for:
  - Security appliances
  - Firewalls

👉 Advanced networking

---

### 4. Classic Load Balancer (Legacy)

- Old generation
- Not recommended

---

## 🧠 Architectural Logic (VERY IMPORTANT)

### Why ELB?

- Distribute traffic
- Improve availability
- Prevent overload

👉 ELB = scalability + reliability

---

## ⚖️ ALB vs NLB (VERY IMPORTANT)

| Feature | ALB | NLB |
|--------|-----|-----|
| Layer | 7 (HTTP) | 4 (TCP/UDP) |
| Routing | Advanced | Basic |
| Use case | Web apps | High performance |

👉 ALB = smart routing  
👉 NLB = raw performance  

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Health Checks (CRITICAL)

- Detect unhealthy instances
- Route traffic only to healthy targets

---

### 2. Auto Scaling Integration

- Works with [[AWS Auto Scaling]]

---

### 3. Multi-AZ Support

- High availability

---

### 4. SSL Termination

- Handles HTTPS

---

## ⚡ Performance & Scaling

- Automatically scales
- Handles millions of requests

---

## 💸 Cost Optimization

- Pay per:
  - Usage
  - Data processed

---

## 🔐 Security (VERY IMPORTANT)

- Security Groups
- SSL/TLS encryption
- Integration with [[AWS WAF]]

---

## 🔄 Integration with Other Services

- [[Amazon EC2]] → compute targets
- [[AWS Auto Scaling]] → dynamic scaling
- [[Amazon CloudWatch]] → monitoring
- [[Amazon Route 53]] → DNS routing

---

## 🚀 Real-World Architecture (Pro Level)

### 🌐 Scalable Web Application

User  
→ ELB (ALB)  
→ Auto Scaling Group (EC2)  
→ Database  

👉 Highly available system

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. ALB = Layer 7 (HTTP/HTTPS)  
👉 Most common

🔥 2. NLB = Layer 4 (TCP/UDP)  
👉 High performance

🔥 3. ELB performs health checks  
👉 Key feature

🔥 4. Key keyword:
> “Distribute traffic / load balancing / high availability”

👉 Answer = ELB

---

## 🧠 Advanced Architect Insight

ELB enables **fault-tolerant architecture**:

Traffic  
→ Load balancer  
→ Healthy instances  

👉 Resilient system

---

## 📊 When NOT to Use ELB

❌ DNS routing → Use [[Amazon Route 53]]  
❌ CDN → Use [[Amazon CloudFront]]  

---

## 🔥 One-Line Summary

👉 ELB = Distributes incoming traffic across multiple resources for high availability

---

## 🔗 Related Services

- Amazon EC2
- AWS Auto Scaling
- Amazon Route 53
- AWS WAF