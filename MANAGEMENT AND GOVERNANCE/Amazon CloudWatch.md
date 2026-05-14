# 🧠 Amazon CloudWatch

## 🔗 Service Type
#Monitoring #Observability #Logging #Metrics

---

## 📌 What is Amazon CloudWatch?

Amazon CloudWatch is a service used to:

- Monitor AWS resources and applications
- Collect metrics, logs, and events
- Trigger automated actions

👉 CloudWatch = “Monitor everything in AWS”

---

## ⚙️ How It Works (Architecture Thinking)

1. Collect data:
   - Metrics (CPU, memory, etc.)
   - Logs (application/system)
   - Events

2. Store and analyze data

3. Trigger actions:
   - Alarms
   - Auto Scaling
   - Lambda functions

👉 Observe → Analyze → Act

---

## 🏗️ Core Components (VERY IMPORTANT)

### 1. Metrics

- Numeric data:
  - CPU utilization
  - Network traffic

---

### 2. Logs

- Application/system logs
- Stored in CloudWatch Logs

---

### 3. Alarms (CRITICAL)

- Trigger actions based on thresholds

Example:
- CPU > 80% → scale out

---

### 4. Dashboards

- Visualize metrics

---

### 5. Events (EventBridge integration)

- React to system events

---

## 🧠 Architectural Logic (Why CloudWatch?)

### When to Choose CloudWatch:

✅ Monitor system performance  
✅ Set alerts (alarms)  
✅ Collect logs  
✅ Trigger automation  

👉 CloudWatch = Monitoring + automation

---

## ⚖️ CloudWatch vs CloudTrail vs X-Ray (VERY IMPORTANT)

| Service | Purpose |
|--------|---------|
| CloudWatch | Metrics + logs |
| CloudTrail | API audit |
| X-Ray | Request tracing |

👉 CloudWatch = “What is happening”  
👉 CloudTrail = “Who did it”  
👉 X-Ray = “Why it happened”  

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Alarms + Auto Scaling

- Trigger scaling actions

---

### 2. Log Monitoring

- Centralized logging

---

### 3. Custom Metrics (IMPORTANT)

- Monitor app-specific data

---

### 4. EventBridge Integration

- Event-driven automation

---

## ⚡ Performance & Scaling

- Fully managed
- Handles large-scale monitoring

---

## 💸 Cost Optimization

- Pay for:
  - Metrics
  - Logs storage
  - Alarms

### Optimize:
- Use log retention policies
- Avoid unnecessary custom metrics

---

## 🔐 Security

- IAM access control
- Encryption support

---

## 🔄 Integration with Other Services

- [[Amazon EC2]] → metrics
- [[AWS Auto Scaling]] → scaling triggers
- [[AWS Lambda]] → automation
- [[Amazon SNS]] → notifications

---

## 🚀 Real-World Architecture (Pro Level)

### 📊 Auto Scaling System

EC2 → CloudWatch metrics  
→ Alarm triggers  
→ Auto Scaling adds instances  

👉 Self-healing system

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. CloudWatch = monitoring ONLY  
👉 Not audit logs

🔥 2. Alarms trigger actions  
👉 Key feature

🔥 3. Logs + metrics both supported  
👉 Important distinction

🔥 4. Key keyword:
> “Monitor / alarms / metrics / logs”

👉 Answer = CloudWatch

---

## 🧠 Advanced Architect Insight

CloudWatch enables **event-driven automation**:

Metric  
→ Alarm  
→ Action  

👉 Reactive systems

---

## 📊 When NOT to Use CloudWatch

❌ Audit logs → Use [[AWS CloudTrail]]  
❌ Trace requests → Use [[AWS X-Ray]]  

---

## 🔥 One-Line Summary

👉 CloudWatch = Monitor metrics, logs, and trigger actions

---

## 🔗 Related Services

- AWS CloudTrail
- AWS X-Ray
- Amazon SNS
- AWS Lambda