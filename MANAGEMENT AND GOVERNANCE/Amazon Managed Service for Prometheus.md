# 🧠 Amazon Managed Service for Prometheus (AMP)

## 🔗 Service Type
#Monitoring #Observability #Metrics #Kubernetes

---

## 📌 What is Amazon Managed Service for Prometheus?

Amazon Managed Service for Prometheus is a **fully managed monitoring service** for:

- Collecting and storing time-series metrics
- Querying metrics using PromQL

👉 AMP = “Managed Prometheus for cloud-native monitoring”

---

## ⚙️ How It Works (Architecture Thinking)

1. Applications (often in [[Amazon EKS]]) generate metrics

2. Prometheus agents scrape metrics

3. Metrics sent to AMP

4. Query using PromQL

5. Visualize using:
   - [[Amazon Managed Grafana]]

👉 Metrics → Storage → Query → Visualization

---

## 🏗️ Core Concepts (VERY IMPORTANT)

### 1. Time-Series Metrics
- Data points over time (CPU, latency, etc.)

---

### 2. PromQL (IMPORTANT)
- Query language for metrics

---

### 3. Workspaces
- Logical containers for metrics

---

### 4. Scraping
- Collecting metrics from services

---

## 🧠 Architectural Logic (Why AMP?)

### When to Choose AMP:

✅ Kubernetes monitoring  
✅ Microservices observability  
✅ Time-series metrics  
✅ Avoid managing Prometheus servers  

👉 AMP = Cloud-native monitoring

---

## ⚖️ AMP vs CloudWatch (VERY IMPORTANT)

| Feature | AMP | CloudWatch |
|--------|-----|------------|
| Focus | Kubernetes metrics | AWS metrics |
| Query | PromQL | CloudWatch queries |
| Use case | Microservices | General monitoring |

👉 CloudWatch = AWS-native  
👉 AMP = Kubernetes-native  

---

## ⚖️ AMP vs Self-Managed Prometheus

| Feature | AMP | Self-managed |
|--------|-----|--------------|
| Management | Fully managed | You manage |
| Scaling | Automatic | Manual |
| Ops effort | Low | High |

👉 AMP = easier + scalable  

---

## ⚡ Key Features (VERY IMPORTANT)

### 1. Fully Managed
- No infrastructure setup

---

### 2. Scalable Metrics Storage
- Handles large workloads

---

### 3. PromQL Support
- Powerful querying

---

### 4. Integration with Grafana
- Visualization layer

---

## ⚡ Performance & Scaling

- High ingestion rate
- Scales automatically

---

## 💸 Cost Optimization

- Pay for:
  - Data ingested
  - Storage
  - Queries

---

## 🔐 Security

- IAM authentication
- VPC endpoints

---

## 🔄 Integration with Other Services

- [[Amazon EKS]] → container metrics
- [[Amazon Managed Grafana]] → dashboards
- [[AWS IAM]] → access control
- [[Amazon CloudWatch]] → complementary monitoring

---

## 🚀 Real-World Architecture (Pro Level)

### 📊 Kubernetes Monitoring System

EKS cluster  
→ Prometheus agents  
→ AMP (metrics storage)  
→ Grafana dashboard  

👉 Full observability stack

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. AMP = metrics ONLY  
👉 Not logs or tracing

🔥 2. Uses PromQL  
👉 Key differentiator

🔥 3. Often used with Grafana  
👉 Visualization combo

🔥 4. Key keyword:
> “Prometheus / Kubernetes metrics / time-series monitoring”

👉 Answer = Amazon Managed Service for Prometheus

---

## 🧠 Advanced Architect Insight

AMP enables **cloud-native observability architecture**:

Metrics  
→ AMP  
→ Grafana  
→ Insights  

👉 Ideal for microservices

---

## 📊 When NOT to Use AMP

❌ General AWS monitoring → Use [[Amazon CloudWatch]]  
❌ Logging → Use CloudWatch Logs  
❌ Tracing → Use [[AWS X-Ray]]  

---

## 🔥 One-Line Summary

👉 AMP = Managed Prometheus service for Kubernetes and time-series metrics

---

## 🔗 Related Services

- Amazon EKS
- Amazon Managed Grafana
- Amazon CloudWatch
- AWS X-Ray