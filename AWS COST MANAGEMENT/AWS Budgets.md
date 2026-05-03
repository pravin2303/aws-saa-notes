# 🧠 AWS Budgets

## 🔗 Service Type
#CostManagement #Monitoring #Alerts #Governance

---

## 📌 What is AWS Budgets?

AWS Budgets is a service that allows you to:

- Set custom cost or usage limits
- Monitor spending in real time
- Receive alerts when thresholds are exceeded

👉 Budgets = “Financial guardrail for AWS usage”

---

## ⚙️ How It Works (Architecture Thinking)

1. Define a budget:
   - Cost (₹/$)
   - Usage (e.g., EC2 hours)
   - Reserved Instance utilization

2. Set threshold:
   - Example: 80%, 100%

3. Configure alerts:
   - Email
   - [[Amazon SNS]]

4. (Optional) Trigger actions:
   - Stop EC2
   - Apply IAM restrictions

👉 Proactive cost control system

---

## 🏗️ Types of Budgets

### 1. Cost Budget
- Monitor total spend

---

### 2. Usage Budget
- Track resource usage (e.g., hours, GB)

---

### 3. Reservation Budget
- Track Reserved Instance utilization

---

### 4. Savings Plans Budget
- Monitor savings plan usage

---

## 🧠 Architectural Logic (Why AWS Budgets?)

### When to Choose Budgets:

✅ Need alerts before overspending  
✅ Want cost control automation  
✅ Monitor team/project spending  
✅ Prevent unexpected bills  

👉 Budgets = Prevent problems (not analyze after)

---

## ⚖️ AWS Budgets vs Cost Explorer (IMPORTANT)

| Feature | AWS Budgets | Cost Explorer |
|--------|------------|---------------|
| Purpose | Alerts & limits | Analysis |
| Timing | Proactive | Reactive |
| Action | Can trigger actions | No actions |

👉 Budgets = Control  
👉 Cost Explorer = Analyze  

---

## ⚡ Key Features (Exam Focus)

### 1. Alerts (VERY IMPORTANT)
- Trigger at threshold (e.g., 80%, 90%)

---

### 2. Budget Actions (HIGH VALUE)

- Stop EC2 instances
- Detach IAM policies
- Restrict usage

👉 Automation for cost control

---

### 3. SNS Integration
- Send alerts to multiple systems

---

## 💸 Cost Optimization Strategy

Use Budgets to:

- Avoid unexpected billing spikes
- Track spending per project
- Enforce cost discipline

---

## 🔐 Security & Governance

- IAM policies control access
- Used in:
  - Multi-account setups
  - Organization-level governance

---

## 🔄 Integration with Other Services

- [[Amazon SNS]] → notifications
- [[AWS Organizations]] → multi-account budgets
- [[AWS Cost Explorer]] → detailed analysis

---

## 🚀 Real-World Architecture (Pro Level)

### 💰 Cost Control System

1. Set monthly budget: ₹5000
2. At 80% → SNS alert sent
3. At 100% → automatic action:
   - Stop EC2 instances

👉 Prevents overspending

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Budgets = proactive  
👉 Alerts BEFORE exceeding

🔥 2. Can trigger actions  
👉 Unique feature

🔥 3. Not for detailed analysis  
👉 Use Cost Explorer

🔥 4. Key keyword:
> “Alert when cost exceeds threshold”

👉 Answer = AWS Budgets

---

## 🧠 Advanced Architect Insight

Budgets is part of **FinOps strategy**:

Monitor  
→ Alert  
→ Act  

👉 Cost governance loop

---

## 📊 When NOT to Use AWS Budgets

❌ Analyze historical trends → Use [[AWS Cost Explorer]]  
❌ Detailed billing reports → Use Cost & Usage Report  

---

## 🔥 One-Line Summary

👉 AWS Budgets = Set limits and get alerts to control AWS costs

---

## 🔗 Related Services

- AWS Cost Explorer
- AWS Cost and Usage Report
- Amazon SNS
- AWS Organizations

# 🔥 Mental Model (Cost Tools)

- Budgets → Alert 🚨
- Cost Explorer → Analyze 📊
- CUR (Cost & Usage Report) → Detailed data 📄