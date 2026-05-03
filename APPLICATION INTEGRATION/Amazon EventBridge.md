# 🧠 Amazon EventBridge

## 🔗 Service Type
#ApplicationIntegration #EventDriven #Serverless #EventBus

---

## 📌 What is Amazon EventBridge?

Amazon EventBridge is a **serverless event bus** that enables applications to:

- Send events
- Route events
- Trigger actions based on events

👉 EventBridge = “If something happens → trigger something else”

---

## ⚙️ How It Works (Architecture Thinking)

1. Event Source generates event:
   - AWS services (EC2, S3, etc.)
   - SaaS apps (via partner integrations)
   - Custom applications

2. Event is sent to EventBridge Bus

3. EventBridge evaluates rules:
   - Match event pattern

4. Target is triggered:
   - [[AWS Lambda]]
   - [[Amazon SQS]]
   - [[Amazon SNS]]
   - [[AWS Step Functions]]

👉 Fully decoupled system

---

## 🏗️ Core Components

### 1. Event Bus
- Default bus (AWS events)
- Custom bus (your apps)
- Partner bus (SaaS integrations)

---

### 2. Rules (VERY IMPORTANT)
- Filter events using JSON patterns
- Route to targets

---

### 3. Targets
- Lambda
- SQS
- SNS
- Step Functions
- Kinesis

---

### 4. Event Schema Registry
- Stores event structure
- Helps developers understand events

---

## 🧠 Architectural Logic (Why EventBridge?)

### When to Choose EventBridge:

✅ Event-driven architecture  
✅ Loose coupling between services  
✅ Trigger workflows automatically  
✅ Integrate AWS + SaaS events  

👉 EventBridge = Central event router

---

## ⚖️ EventBridge vs SNS vs SQS (VERY IMPORTANT)

### EventBridge vs SNS

| Feature | EventBridge | SNS |
|--------|------------|-----|
| Routing | Advanced (rules) | Simple |
| Filtering | Content-based | Limited |
| Use case | Complex workflows | Notifications |

👉 SNS = Broadcast  
👉 EventBridge = Smart routing  

---

### EventBridge vs SQS

| Feature | EventBridge | SQS |
|--------|------------|-----|
| Type | Event bus | Queue |
| Pattern | Push-based | Pull-based |
| Use case | Event routing | Decoupling |

👉 SQS = Buffer  
👉 EventBridge = Router  

---

## ⚡ Performance & Scaling

- Fully serverless
- Automatically scales
- Handles high event throughput

---

## 💸 Cost Optimization

- Pay per:
  - Number of events processed

### Reduce cost:
- Filter events efficiently (rules)
- Avoid unnecessary triggers

---

## 🔐 Security

- IAM policies control access
- Event bus permissions
- Encryption in transit (HTTPS)

---

## 🔄 Integration with Other Services

- [[AWS Lambda]] → compute
- [[Amazon SQS]] → queue
- [[Amazon SNS]] → notifications
- [[AWS Step Functions]] → workflows
- [[Amazon Kinesis]] → streaming

---

## 🚀 Real-World Architecture (Pro Level)

### 📦 E-commerce Order System

1. Order placed → event generated
2. EventBridge receives event
3. Rules trigger:
   - Lambda → process payment
   - SNS → send notification
   - SQS → queue order processing

👉 Fully decoupled microservices

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. EventBridge = event routing (NOT storage)  
👉 Does not store events long-term

🔥 2. Content-based filtering  
👉 Strong advantage over SNS

🔥 3. Supports SaaS integrations  
👉 Unique feature

🔥 4. Key keyword:
> “Event-driven architecture / loosely coupled services”

👉 Answer = EventBridge

---

## 🧠 Advanced Architect Insight

EventBridge enables **event-driven microservices**:

Service A → EventBridge → Service B / C / D  

👉 No direct communication → loose coupling

---

## 📊 When NOT to Use EventBridge

❌ Need message durability → Use [[Amazon SQS]]  
❌ Simple notifications → Use [[Amazon SNS]]  
❌ Streaming data → Use [[Amazon Kinesis]]  

---

## 🔥 One-Line Summary

👉 EventBridge = Serverless event bus for routing events across AWS services

---

## 🔗 Related Services

- Amazon SQS
- Amazon SNS
- AWS Lambda
- AWS Step Functions
- Amazon Kinesis