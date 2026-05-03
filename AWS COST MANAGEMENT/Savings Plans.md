# 🧠 AWS Savings Plans

## 🔗 Service Type
#CostManagement #Pricing #Optimization #FinOps

---

## 📌 What are Savings Plans?

Savings Plans are a **flexible pricing model** that provide **discounts (up to ~72%)** in exchange for a **commitment to a consistent amount of usage ($/hour)** over 1 or 3 years.

👉 Savings Plans = “Commit usage → get discount”

---

## ⚙️ How It Works (Architecture Thinking)

1. Commit to spend:
   - Example: $10/hour

2. AWS automatically applies discounts to eligible usage

3. Any usage above commitment → billed at On-Demand rate

👉 No need to reserve specific instances

---

## 🏗️ Types of Savings Plans (VERY IMPORTANT)

### 1. Compute Savings Plan (MOST FLEXIBLE)

- Applies to:
  - [[Amazon EC2]]
  - [[AWS Lambda]]
  - [[AWS Fargate]]

- Flexibility:
  - Any region
  - Any instance type
  - Any OS

👉 Best for most use cases

---

### 2. EC2 Instance Savings Plan

- Applies only to EC2

- Limited flexibility:
  - Specific region
  - Instance family

👉 Higher discount than Compute SP

---

## 🧠 Architectural Logic (Why Savings Plans?)

### When to Choose Savings Plans:

✅ Predictable usage over time  
✅ Want cost reduction without losing flexibility  
✅ Long-running workloads  

👉 Savings Plans = Default cost optimization strategy

---

## ⚖️ Savings Plans vs Reserved Instances (VERY IMPORTANT)

| Feature | Savings Plans | Reserved Instances |
|--------|-------------|--------------------|
| Flexibility | High | Low |
| Coverage | EC2 + Lambda + Fargate | Mostly EC2 |
| Management | Automatic | Manual |
| Recommendation | Preferred | Legacy option |

👉 Exam logic:
- Modern → Savings Plans  
- Old / strict control → RI  

---

## ⚡ Types of Payment Options

- No upfront
- Partial upfront
- All upfront

👉 More upfront = more discount

---

## 💸 Cost Optimization Strategy

### Use Savings Plans for:
- Steady workloads
- Production systems
- Always-running services

---

### Combine with:
- [[Amazon EC2 Spot Instances]] → for variable workloads
- On-Demand → for unpredictable usage

---

## 🔐 Governance

- Managed via AWS Billing
- Integrated with:
  - [[AWS Cost Explorer]]
  - [[AWS Budgets]]

---

## 🔄 Integration with Other Services

- Amazon EC2
- AWS Lambda
- AWS Fargate
- AWS Cost Explorer
- AWS Budgets

---

## 🚀 Real-World Architecture (Pro Level)

### 💰 Cost Optimization Strategy

1. Analyze usage using Cost Explorer
2. Identify steady baseline usage
3. Purchase Savings Plan
4. Use On-Demand for spikes
5. Use Spot Instances for extra savings

👉 Hybrid pricing strategy

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Savings Plans = flexible commitment  
👉 Not tied to instance type

🔥 2. Compute SP covers multiple services  
👉 EC2 + Lambda + Fargate

🔥 3. Best default recommendation  
👉 Often correct answer

🔥 4. Key keyword:
> “Reduce cost with flexibility / predictable workload”

👉 Answer = Savings Plans

---

## 🧠 Advanced Architect Insight

Savings Plans are part of **cost optimization pillar**:

Baseline usage → Savings Plans  
Spiky usage → Spot  
Unpredictable → On-Demand  

---

## 📊 When NOT to Use Savings Plans

❌ Short-term workloads  
❌ Unpredictable usage  
❌ Testing environments  

---

## 🔥 One-Line Summary

👉 Savings Plans = Flexible discount model for predictable AWS usage

---

## 🔗 Related Services

- Amazon EC2
- AWS Lambda
- AWS Fargate
- AWS Cost Explorer
- AWS Budgets