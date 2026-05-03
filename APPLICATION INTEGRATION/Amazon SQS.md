# 🧠 Amazon SQS (Simple Queue Service)

## 🔗 Service Type
#ApplicationIntegration #Queue #Decoupling #Serverless

---

## 📌 What is Amazon SQS?

Amazon SQS is a **fully managed message queue service** that allows applications to:

- Send messages
- Store messages
- Process messages asynchronously

👉 SQS = “Buffer between components”

---

## ⚙️ How It Works (Architecture Thinking)

1. Producer sends message to queue
2. Message stored in SQS
3. Consumer pulls message (polling)
4. Message processed and deleted

👉 Pull-based system (not push)

---

## 🏗️ Core Concepts (VERY IMPORTANT)

### 1. Queue
- Temporary storage for messages

---

### 2. Message
- Data (up to 256 KB)

---

### 3. Visibility Timeout (CRITICAL)

- Message becomes invisible after being read
- Prevents duplicate processing

👉 If not deleted → message reappears

---

### 4. Long Polling
- Reduces empty responses
- Improves efficiency

---

## 🧠 Types of SQS

### 1. Standard Queue

- Unlimited throughput
- At-least-once delivery
- Best-effort ordering

👉 Use for most applications

---

### 2. FIFO Queue

- Exactly-once processing
- Strict ordering

👉 Use when order matters

---

## 🧠 Architectural Logic (Why SQS?)

### When to Choose SQS:

✅ Decouple microservices  
✅ Handle traffic spikes  
✅ Ensure message durability  
✅ Asynchronous processing  

👉 SQS = Reliability + Scalability

---

## ⚖️ SQS vs SNS vs EventBridge (VERY IMPORTANT)

### SQS vs SNS

| Feature | SQS | SNS |
|--------|-----|-----|
| Pattern | Queue | Pub/Sub |
| Delivery | Pull | Push |
| Use case | Buffer | Broadcast |

👉 SQS = Store  
👉 SNS = Send  

---

### SQS vs EventBridge

| Feature | SQS | EventBridge |
|--------|-----|-------------|
| Role | Queue | Event router |
| Delivery | Pull | Push |
| Use case | Reliability | Routing |

---

## ⚡ Performance & Scaling

- Fully serverless
- Auto scales
- Supports high throughput

---

## 💸 Cost Optimization

- Pay per:
  - Requests
  - Data transfer

### Reduce cost:
- Use long polling
- Batch messages

---

## 🔐 Security

- IAM policies
- Queue policies
- Encryption:
  - At rest (KMS)
  - In transit (HTTPS)

---

## 🔄 Integration with Other Services

- [[AWS Lambda]] → event processing
- [[Amazon SNS]] → fan-out pattern
- [[Amazon EventBridge]] → event routing
- [[Amazon EC2]] → consumers

---

## 🚀 Real-World Architecture (Pro Level)

### 📦 Order Processing System

1. User places order
2. Order sent to SQS
3. Worker service processes order
4. If failure → message retries

👉 Handles spikes + ensures reliability

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. SQS = pull-based  
👉 Consumer must poll

🔥 2. Message durability  
👉 Stored until processed

🔥 3. Duplicate messages possible  
👉 Handle idempotency

🔥 4. Key keyword:
> “Decouple services / handle spikes / queue messages”

👉 Answer = SQS

---

## 🧠 Advanced Architect Insight

SQS enables **loosely coupled systems**:

Producer  
→ SQS Queue  
→ Consumer  

👉 Independent scaling

---

## 📊 When NOT to Use SQS

❌ Broadcast messages → Use [[Amazon SNS]]  
❌ Event routing → Use [[Amazon EventBridge]]  
❌ Real-time streaming → Use [[Amazon Kinesis]]  

---

## 🔥 One-Line Summary

👉 SQS = Reliable, scalable message queue for decoupling systems

---

## 🔗 Related Services

- Amazon SNS
- Amazon EventBridge
- AWS Lambda
- Amazon EC2