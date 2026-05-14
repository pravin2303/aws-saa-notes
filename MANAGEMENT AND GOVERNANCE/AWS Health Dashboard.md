# 🧠 AWS Health Dashboard

## 🔗 Service Type
#Monitoring #Operations #Status #Notifications

---

## 📌 What is AWS Health Dashboard?

AWS Health Dashboard provides:

- Real-time information about AWS service health
- Alerts for issues affecting your AWS resources
- Personalized notifications

👉 Health Dashboard = “AWS service status + impact on your account”

---

## ⚙️ How It Works (Architecture Thinking)

1. AWS detects issue:
   - Service outage
   - Maintenance event

2. Health Dashboard shows:
   - Affected services
   - Regions
   - Resources

3. Sends notifications:
   - Email
   - [[Amazon SNS]]

👉 Awareness of AWS-side issues

---

## 🏗️ Core Components (VERY IMPORTANT)

### 1. Service Health Dashboard (Public)

- Global AWS service status
- No account-specific details

---

### 2. Personal Health Dashboard (CRITICAL)

- Account-specific issues
- Resource-level impact

---

## 🧠 Architectural Logic (Why Health Dashboard?)

### When to Use:

✅ AWS service outages  
✅ Maintenance notifications  
✅ Account-specific issues  
✅ Operational awareness  

👉 Health Dashboard = AWS-side visibility

---

## ⚖️ Health Dashboard vs CloudWatch vs CloudTrail (VERY IMPORTANT)

| Service | Purpose |
|--------|---------|
| Health Dashboard | AWS service issues |
| CloudWatch | Resource monitoring |
| CloudTrail | API auditing |

👉 Health = “AWS problem”  
👉 CloudWatch = “Your system problem”  

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Real-Time Alerts
- Immediate updates on issues

---

### 2. Account-Specific Insights
- Shows impacted resources

---

### 3. Scheduled Maintenance Notifications
- Planned updates

---

### 4. Integration with EventBridge (IMPORTANT)

- Trigger automated responses

---

## ⚡ High Availability

- Fully managed
- Global service visibility

---

## 💸 Cost Optimization

- Free service

---

## 🔐 Security

- IAM-controlled access

---

## 🔄 Integration with Other Services

- [[Amazon EventBridge]] → event-driven actions
- [[Amazon SNS]] → notifications
- [[AWS Lambda]] → automated responses

---

## 🚀 Real-World Architecture (Pro Level)

### 🚨 Incident Response System

AWS issue detected  
→ Health Dashboard event  
→ EventBridge triggers Lambda  
→ Notify team via SNS  

👉 Automated incident response

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Health Dashboard = AWS issues ONLY  
👉 Not your app monitoring

🔥 2. Personal dashboard = account-specific  
👉 Key difference

🔥 3. Works with EventBridge  
👉 Automation use case

🔥 4. Key keyword:
> “AWS service outage / maintenance / account impact”

👉 Answer = AWS Health Dashboard

---

## 🧠 Advanced Architect Insight

Health Dashboard enables **proactive incident awareness**:

AWS issue  
→ Notification  
→ Action  

👉 Improves reliability

---

## 📊 When NOT to Use Health Dashboard

❌ Monitor CPU → Use [[Amazon CloudWatch]]  
❌ Audit API calls → Use [[AWS CloudTrail]]  

---

## 🔥 One-Line Summary

👉 AWS Health Dashboard = Monitor AWS service health and account-specific issues

---

## 🔗 Related Services

- Amazon CloudWatch
- AWS CloudTrail
- Amazon EventBridge
- Amazon SNS