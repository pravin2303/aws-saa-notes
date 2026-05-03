# 🧠 AWS Step Functions

## 🔗 Service Type
#ApplicationIntegration #Orchestration #Workflow #Serverless

---

## 📌 What is AWS Step Functions?

AWS Step Functions is a **serverless workflow orchestration service** used to:

- Coordinate multiple AWS services
- Define workflows as state machines
- Handle retries, errors, and branching

👉 Step Functions = “Control flow for your architecture”

---

## ⚙️ How It Works (Architecture Thinking)

1. Define workflow using **State Machine (JSON/YAML)**
2. Each step (state) performs an action:
   - [[AWS Lambda]]
   - [[Amazon SQS]]
   - [[Amazon SNS]]
   - [[Amazon ECS]]
   - [[AWS Glue]]

3. Workflow executes step-by-step:
   - Sequential
   - Parallel
   - Conditional branching

👉 Visual + controlled execution

---

## 🏗️ Core Concepts

### 1. State Machine (VERY IMPORTANT)
- Defines workflow logic
- Written in Amazon States Language (ASL)

---

### 2. States

- **Task** → perform work (Lambda, etc.)
- **Choice** → branching logic
- **Parallel** → run tasks simultaneously
- **Wait** → delay execution
- **Fail / Succeed** → end states

---

### 3. Execution
- Instance of workflow run

---

## 🧠 Architectural Logic (Why Step Functions?)

### When to Choose Step Functions:

✅ Multi-step workflows  
✅ Need retries & error handling  
✅ Conditional logic (if/else)  
✅ Long-running processes  
✅ Microservices orchestration  

👉 Step Functions = Workflow engine

---

## ⚖️ Step Functions vs Other Services (VERY IMPORTANT)

### Step Functions vs Lambda

| Feature | Step Functions | Lambda |
|--------|--------------|--------|
| Role | Orchestration | Execution |
| Logic | Workflow control | Code execution |
| Use case | Multi-step flows | Single task |

👉 Lambda = Worker  
👉 Step Functions = Manager  

---

### Step Functions vs EventBridge

| Feature | Step Functions | EventBridge |
|--------|--------------|-------------|
| Pattern | Workflow | Event routing |
| Control | High | Low |
| Use case | Sequential logic | Trigger events |

👉 EventBridge = Trigger  
👉 Step Functions = Process  

---

## ⚡ Workflow Types

### 1. Standard Workflows
- Long-running (up to 1 year)
- Durable
- Exactly-once execution

👉 Use for business workflows

---

### 2. Express Workflows
- High throughput
- Short duration
- Lower cost

👉 Use for high-volume events

---

## ⚡ Performance & Scaling

- Fully serverless
- Scales automatically
- Handles thousands of executions

---

## 💸 Cost Optimization

- Pay per:
  - State transitions

### Reduce cost:
- Optimize workflow steps
- Use Express for high-volume workloads

---

## 🔐 Security

- IAM roles for execution
- Service permissions
- Encryption in transit

---

## 🔄 Integration with Other Services

- [[AWS Lambda]] → compute
- [[Amazon SQS]] → queue
- [[Amazon SNS]] → notifications
- [[AWS Glue]] → ETL
- [[Amazon ECS]] → containers
- [[Amazon EventBridge]] → triggers

---

## 🚀 Real-World Architecture (Pro Level)

### 📦 Order Processing Workflow

1. Order placed → EventBridge triggers Step Function
2. Step 1 → Validate order (Lambda)
3. Step 2 → Process payment
4. Step 3 → Update database
5. Step 4 → Send notification (SNS)

👉 Fully automated workflow with retries

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Step Functions = orchestration (NOT compute)  
👉 Uses Lambda/others to execute

🔥 2. Built-in retry & error handling  
👉 Big advantage

🔥 3. Visual workflows  
👉 Debugging easier

🔥 4. Key keyword:
> “Multi-step workflow / orchestration / retry logic”

👉 Answer = Step Functions

---

## 🧠 Advanced Architect Insight

Step Functions enables **microservices orchestration**:

Event → Step Function  
→ Multiple services (Lambda, SQS, etc.)  
→ Controlled execution  

👉 Replaces complex custom code

---

## 📊 When NOT to Use Step Functions

❌ Simple event trigger → Use [[Amazon EventBridge]]  
❌ Single task → Use [[AWS Lambda]]  
❌ Streaming pipelines → Use [[Amazon Kinesis]]  

---

## 🔥 One-Line Summary

👉 Step Functions = Serverless workflow engine for orchestrating AWS services

---

## 🔗 Related Services

- AWS Lambda
- Amazon EventBridge
- Amazon SQS
- Amazon SNS
- AWS Glue
- Amazon ECS