# 🧠 AWS Lambda

## 🔗 Service Type
#Compute #Serverless #EventDriven #Scaling

---

## 📌 What is AWS Lambda?

AWS Lambda is a service that:

- Runs code without managing servers
- Executes code in response to events

👉 Lambda = “Run code on demand (serverless)”

---

## ⚙️ How It Works (Architecture Thinking)

1. Upload code

2. Configure trigger:
   - [[Amazon S3]]
   - [[Amazon API Gateway]]
   - [[Amazon EventBridge]]

3. Event triggers function

4. Lambda executes code

👉 Event → Lambda → Execute → Response

---

## 🏗️ Core Concepts (VERY IMPORTANT)

### 1. Function

- Your code

---

### 2. Trigger (CRITICAL)

- Event source:
  - S3 upload
  - HTTP request
  - Schedule

---

### 3. Execution Role

- IAM role for permissions

---

### 4. Stateless Execution

- No persistent state

---

## 🧠 Architectural Logic (VERY IMPORTANT)

### When to Use Lambda:

✅ Event-driven workloads  
✅ Microservices  
✅ Backend APIs  
✅ Automation tasks  

👉 Lambda = serverless compute

---

## ⚖️ Lambda vs EC2 (VERY IMPORTANT)

| Feature | Lambda | EC2 |
|--------|--------|-----|
| Server management | None | Required |
| Scaling | Automatic | Manual/ASG |
| Billing | Per execution | Per hour |

👉 Lambda = serverless  
👉 EC2 = full control  

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Event-Driven (CRITICAL)
- Runs only when triggered

---

### 2. Auto Scaling
- Handles thousands of requests

---

### 3. Pay Per Use
- No idle cost

---

### 4. Stateless
- No data persistence

---

## ⚡ Performance & Scaling

- Scales automatically
- Cold start latency (IMPORTANT)

---

## 💸 Cost Optimization

- Pay for:
  - Execution time
  - Requests

---

## 🔐 Security (VERY IMPORTANT)

- IAM execution roles
- VPC integration

---

## 🔄 Integration with Other Services

- [[Amazon API Gateway]] → APIs
- [[Amazon S3]] → file processing
- [[Amazon DynamoDB]] → data storage
- [[Amazon EventBridge]] → event routing

---

## 🚀 Real-World Architecture (Pro Level)

### ⚡ Serverless API

User  
→ API Gateway  
→ Lambda  
→ DynamoDB  

👉 Fully serverless system

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Lambda = stateless  
👉 No local storage

🔥 2. Cold start exists  
👉 Performance consideration

🔥 3. Max execution time = 15 minutes  
👉 Important limit

🔥 4. Key keyword:
> “Event-driven / no servers / automatic scaling”

👉 Answer = AWS Lambda

---

## 🧠 Advanced Architect Insight

Lambda enables **event-driven architecture**:

Event  
→ Lambda  
→ Action  

👉 Scalable + cost-efficient

---

## 📊 When NOT to Use Lambda

❌ Long-running tasks → Use EC2  
❌ Stateful apps → Use containers  

---

## 🔥 One-Line Summary

👉 AWS Lambda = Run code without servers in response to events

---

## 🔗 Related Services

- Amazon API Gateway
- Amazon S3
- Amazon DynamoDB
- Amazon EventBridge