# 🧠 Amazon EC2 Auto Scaling

## 🔗 Service Type
#Compute #AutoScaling #HighAvailability #Elasticity

---

## 📌 What is EC2 Auto Scaling?

Amazon EC2 Auto Scaling automatically:

- Launches EC2 instances
- Terminates EC2 instances
- Maintains desired capacity

👉 Auto Scaling = “Right number of servers at the right time”

---

## ⚙️ How It Works (Architecture Thinking)

1. Define Auto Scaling Group (ASG)
2. Set:
   - Minimum instances
   - Desired instances
   - Maximum instances
3. Attach scaling policies
4. Monitor via [[Amazon CloudWatch]]

👉 Fully automated scaling system

---

## 🏗️ Core Components (VERY IMPORTANT)

### 1. Auto Scaling Group (ASG)

- Logical group of EC2 instances
- Maintains desired capacity

---

### 2. Launch Template / Launch Configuration

- Defines:
  - AMI
  - Instance type
  - Security groups

---

### 3. Scaling Policies

#### a. Target Tracking (MOST COMMON)
- Example:
  - Keep CPU at 50%

---

#### b. Step Scaling
- Scale based on thresholds

---

#### c. Scheduled Scaling
- Scale at specific times

---

## 🧠 Architectural Logic (Why Auto Scaling?)

### When to Choose Auto Scaling:

✅ Traffic varies over time  
✅ Need high availability  
✅ Want cost optimization  
✅ Avoid manual scaling  

👉 Auto Scaling = Elastic + resilient systems

---

## ⚖️ Auto Scaling vs Manual Scaling

| Feature | Auto Scaling | Manual |
|--------|-------------|--------|
| Efficiency | High | Low |
| Cost | Optimized | Risky |
| Reliability | High | Low |

👉 Always prefer Auto Scaling

---

## ⚡ Scaling Types (VERY IMPORTANT)

### 1. Dynamic Scaling
- Based on metrics (CPU, requests)

---

### 2. Predictive Scaling
- Uses ML to predict traffic

---

### 3. Scheduled Scaling
- Predefined time-based scaling

---

## ⚡ High Availability (CRITICAL)

- Deploy across multiple AZs
- Automatically replaces failed instances

👉 Self-healing system

---

## 💸 Cost Optimization

- Scale in when demand is low
- Use Spot Instances in ASG

👉 Pay only for what you use

---

## 🔐 Security

- IAM roles
- Security groups applied via launch template

---

## 🔄 Integration with Other Services

- [[Amazon EC2]] → compute
- [[Elastic Load Balancing]] → distribute traffic
- [[Amazon CloudWatch]] → metrics & alarms
- [[Amazon SNS]] → notifications

---

## 🚀 Real-World Architecture (Pro Level)

### 🌐 Scalable Web Application

1. Users → Load Balancer
2. Load Balancer → ASG (EC2 instances)
3. Auto Scaling adjusts instances based on traffic

👉 Handles traffic spikes automatically

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Auto Scaling = maintains desired capacity  
👉 Replaces failed instances automatically

🔥 2. Works best with Load Balancer  
👉 Common exam pattern

🔥 3. Multi-AZ deployment is key  
👉 High availability

🔥 4. Key keyword:
> “Automatically scale based on demand”

👉 Answer = Auto Scaling

---

## 🧠 Advanced Architect Insight

Auto Scaling enables **elastic architecture**:

Low traffic → fewer instances  
High traffic → more instances  

👉 Optimal performance + cost

---

## 📊 When NOT to Use Auto Scaling

❌ Fixed workload → Use single EC2  
❌ Event-driven compute → Use [[AWS Lambda]]  

---

## 🔥 One-Line Summary

👉 Auto Scaling = Automatically adjust EC2 capacity based on demand

---

## 🔗 Related Services

- Amazon EC2
- Elastic Load Balancing
- Amazon CloudWatch
- Amazon SNS