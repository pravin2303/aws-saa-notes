# 🧠 Amazon API Gateway

## 🔗 Service Type
#ApplicationIntegration #Serverless #API #Microservices

---

## 📌 What is Amazon API Gateway?

Amazon API Gateway is a **fully managed service** to:

- Create, publish, and manage APIs
- Secure APIs
- Handle traffic at scale

👉 API Gateway = “Front door for applications”

---

## ⚙️ How It Works (Architecture Thinking)

Client → API Gateway → Backend service

Backends can be:
- [[AWS Lambda]]
- [[Amazon EC2]]
- [[Amazon ECS]]
- [[AWS Step Functions]]

👉 Acts as entry point + traffic manager

---

## 🏗️ API Types (VERY IMPORTANT)

### 1. REST API
- Full features
- API keys, caching, throttling

---

### 2. HTTP API (MOST USED)

- Lower cost
- Faster performance
- Limited features

---

### 3. WebSocket API

- Real-time communication
- Chat apps, live updates

---

## 🧠 Architectural Logic (Why API Gateway?)

### When to Choose API Gateway:

✅ Build serverless APIs  
✅ Expose microservices  
✅ Secure API endpoints  
✅ Handle high traffic  

👉 API Gateway = API management layer

---

## ⚖️ API Gateway vs ALB (VERY IMPORTANT)

| Feature | API Gateway | ALB |
|--------|-------------|-----|
| Type | API management | Load balancer |
| Features | Auth, throttling, caching | Routing only |
| Use case | Serverless APIs | EC2/ECS apps |

👉 API Gateway = smart entry  
👉 ALB = traffic routing  

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Authentication & Authorization

- IAM
- [[Amazon Cognito]]
- Lambda authorizers

---

### 2. Throttling

- Limit requests
- Prevent abuse

---

### 3. Caching

- Reduce backend load
- Improve performance

---

### 4. Request/Response Transformation

- Modify requests before backend

---

### 5. Rate Limiting

- Protect APIs

---

## ⚡ Performance & Scaling

- Fully serverless
- Automatically scales

👉 Handles millions of requests

---

## 💸 Cost Optimization

- Pay per API call

### Optimize:
- Use caching
- Use HTTP APIs (cheaper)

---

## 🔐 Security

- IAM roles
- Cognito auth
- WAF integration

---

## 🔄 Integration with Other Services

- [[AWS Lambda]] → serverless compute
- [[Amazon Cognito]] → authentication
- [[AWS WAF]] → security
- [[Amazon CloudWatch]] → monitoring

---

## 🚀 Real-World Architecture (Pro Level)

### 🌐 Serverless API

Client → API Gateway  
→ Lambda  
→ DynamoDB  

👉 Fully serverless backend

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. API Gateway = NOT compute  
👉 It routes requests

🔥 2. Built-in security + throttling  
👉 Key advantage

🔥 3. Works best with Lambda  
👉 Common pattern

🔥 4. Key keyword:
> “Expose API / secure endpoints / serverless API”

👉 Answer = API Gateway

---

## 🧠 Advanced Architect Insight

API Gateway enables **decoupled architectures**:

Client  
→ API Gateway  
→ Microservices  

👉 Loose coupling

---

## 📊 When NOT to Use API Gateway

❌ Simple load balancing → Use [[Elastic Load Balancing]]  
❌ Internal-only traffic → Use ALB  

---

## 🔥 One-Line Summary

👉 API Gateway = Managed service to create, secure, and scale APIs

---

## 🔗 Related Services

- AWS Lambda
- Amazon Cognito
- AWS WAF
- Amazon CloudWatch