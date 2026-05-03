# 🧠 AWS Batch

## 🔗 Service Type
#Compute #BatchProcessing #Containers #ServerlessCompute

---

## 📌 What is AWS Batch?

AWS Batch is a service that enables you to **run batch computing jobs at scale** without managing infrastructure.

👉 Automatically:
- Provisions compute resources
- Schedules jobs
- Scales workloads

👉 Batch = “Run large jobs efficiently in the background”

---

## ⚙️ How It Works (Architecture Thinking)

1. Define Job
2. Submit Job to Job Queue
3. AWS Batch schedules job
4. Runs job on:
   - [[Amazon EC2]]
   - [[AWS Fargate]]

5. Output stored in:
   - [[Amazon S3]]
   - Databases

👉 Fully managed job execution pipeline

---

## 🏗️ Core Components (VERY IMPORTANT)

### 1. Job Definition
- Defines:
  - Container image
  - CPU / memory
  - Environment

---

### 2. Job Queue
- Holds submitted jobs
- Prioritizes execution

---

### 3. Compute Environment
- Provides compute resources:
  - EC2 (including Spot)
  - Fargate (serverless)

---

## 🧠 Architectural Logic (Why AWS Batch?)

### When to Choose AWS Batch:

✅ Large-scale batch processing  
✅ Jobs that can run asynchronously  
✅ Compute-heavy workloads  
✅ Need automatic scaling  

👉 Batch = Efficient background processing

---

## ⚖️ AWS Batch vs Other Services (VERY IMPORTANT)

### Batch vs Lambda

| Feature | AWS Batch | Lambda |
|--------|----------|--------|
| Duration | Long-running | Max ~15 min |
| Workload | Heavy compute | Lightweight |
| Control | High | Limited |

👉 Lambda = short tasks  
👉 Batch = long heavy jobs  

---

### Batch vs ECS/Fargate

| Feature | AWS Batch | ECS/Fargate |
|--------|----------|-------------|
| Scheduling | Built-in | Manual |
| Use case | Batch jobs | Services/apps |
| Scaling | Automatic | Configurable |

👉 Batch = job scheduler  
👉 ECS = container platform  

---

## ⚡ Performance & Scaling

- Automatically scales compute resources
- Uses Spot Instances for cost savings

👉 High efficiency for large workloads

---

## 💸 Cost Optimization (VERY IMPORTANT)

- Pay for:
  - EC2 / Fargate usage

### Reduce cost:
- Use Spot Instances (huge savings)
- Optimize job queue priorities
- Use Fargate for simplicity

---

## 🔐 Security

- IAM roles for jobs
- VPC integration
- Encryption via underlying services

---

## 🔄 Integration with Other Services

- [[Amazon S3]] → input/output storage
- [[AWS Lambda]] → trigger jobs
- [[Amazon CloudWatch]] → logs
- [[Amazon ECS]] → container execution

---

## 🚀 Real-World Architecture (Pro Level)

### 📊 Data Processing Pipeline

1. Data stored in S3
2. Batch job triggered
3. Batch processes data (ETL / ML)
4. Output stored in S3 or Redshift

👉 Large-scale data processing

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Batch is NOT real-time  
👉 It is asynchronous

🔥 2. Uses containers  
👉 Runs on ECS/Fargate

🔥 3. Supports Spot Instances  
👉 Key cost optimization point

🔥 4. Key keyword:
> “Batch processing / long-running jobs / queue-based compute”

👉 Answer = AWS Batch

---

## 🧠 Advanced Architect Insight

Batch is used in **data-heavy compute pipelines**:

S3  
→ AWS Batch  
→ S3 / Redshift  

👉 Efficient compute layer

---

## 📊 When NOT to Use AWS Batch

❌ Real-time processing → Use [[AWS Lambda]]  
❌ Continuous services → Use [[Amazon ECS]]  
❌ Streaming workloads → Use [[Amazon Kinesis]]  

---

## 🔥 One-Line Summary

👉 AWS Batch = Managed service for running large-scale batch jobs efficiently

---

## 🔗 Related Services

- Amazon EC2
- AWS Fargate
- Amazon ECS
- Amazon S3
- AWS Lambda