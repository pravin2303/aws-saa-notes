# 🧠 Amazon SNS (Simple Notification Service)

## 🔗 Service Type
#ApplicationIntegration #PubSub #Messaging #Serverless

---

## 📌 What is Amazon SNS?

Amazon SNS is a **fully managed Pub/Sub (publish-subscribe) messaging service** used to:

- Send messages to multiple subscribers
- Broadcast notifications

👉 SNS = “One-to-many message delivery”

---

## ⚙️ How It Works (Architecture Thinking)

1. Publisher sends message to SNS Topic

2. SNS distributes message to all subscribers:

   - [[Amazon SQS]]
   - [[AWS Lambda]]
   - HTTP/HTTPS endpoints
   - Email / SMS

👉 Push-based delivery (instant)

---

## 🏗️ Core Components

### 1. Topic (VERY IMPORTANT)
- Logical communication channel
- Producers publish messages here

---

### 2. Publishers
- Applications / services sending messages

---

### 3. Subscribers
- Services receiving messages

---

## 🧠 Architectural Logic (Why SNS?)

### When to Choose SNS:

✅ Need to send message to multiple services  
✅ Event fan-out pattern  
✅ Real-time notifications  
✅ Decoupled architecture  

👉 SNS = Broadcast system

---

## ⚖️ SNS vs SQS vs EventBridge (VERY IMPORTANT)

### SNS vs SQS

| Feature | SNS | SQS |
|--------|-----|-----|
| Pattern | Pub/Sub | Queue |
| Delivery | Push | Pull |
| Use case | Broadcast | Buffer |

👉 SNS = Fan-out  
👉 SQS = Buffer  

---

### SNS vs EventBridge

| Feature | SNS | EventBridge |
|--------|-----|-------------|
| Routing | Simple | Advanced |
| Filtering | Basic | Content-based |
| Use case | Notifications | Event routing |

👉 SNS = Simple broadcast  
👉 EventBridge = Smart routing  

---

## ⚡ Message Delivery Types

### 1. Standard Topics
- High throughput
- Best-effort ordering

### 2. FIFO Topics
- Ordered delivery
- Exactly-once processing

👉 Used when order matters

---

## ⚡ Performance & Scaling

- Fully serverless
- Automatically scales
- Handles millions of messages

---

## 💸 Cost Optimization

- Pay per:
  - Messages published
  - Data transfer

### Reduce cost:
- Filter messages
- Avoid unnecessary subscriptions

---

## 🔐 Security

- IAM policies
- Topic policies
- Encryption (KMS)
- HTTPS endpoints

---

## 🔄 Integration with Other Services

- [[Amazon SQS]] → queue subscribers
- [[AWS Lambda]] → event processing
- [[Amazon EventBridge]] → event routing
- [[Amazon EC2]] → applications

---

## 🚀 Real-World Architecture (Pro Level)

### 📦 Order Notification System

1. Order placed
2. SNS Topic receives event
3. SNS fans out to:
   - Lambda → process order
   - SQS → queue processing
   - Email → notify user

👉 One event → multiple actions

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. SNS = push-based  
👉 Not pull like SQS

🔥 2. No message storage  
👉 If consumer fails → message lost (unless SQS used)

🔥 3. Fan-out pattern is key  
👉 SNS → multiple SQS queues

🔥 4. Key keyword:
> “Send message to multiple services”

👉 Answer = SNS

---

## 🧠 Advanced Architect Insight

SNS enables **fan-out architecture**:

Producer  
→ SNS Topic  
→ Multiple Subscribers (Lambda, SQS, etc.)

👉 Highly scalable and decoupled

---

## 📊 When NOT to Use SNS

❌ Need message durability → Use [[Amazon SQS]]  
❌ Complex event filtering → Use [[Amazon EventBridge]]  
❌ Message replay needed → Use SQS  

---

## 🔥 One-Line Summary

👉 SNS = Pub/Sub service for broadcasting messages to multiple subscribers

---

## 🔗 Related Services

- Amazon SQS
- Amazon EventBridge
- AWS Lambda
- Amazon EC2