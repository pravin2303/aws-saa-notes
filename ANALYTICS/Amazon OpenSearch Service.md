# 🧠 Amazon OpenSearch Service

## 🔗 Service Type
#Analytics #Search #LogAnalytics #RealTime

---

## 📌 What is Amazon OpenSearch Service?

Amazon OpenSearch Service is a **managed search and analytics engine** used for:

- Full-text search
- Log analytics
- Real-time monitoring

👉 Based on:
- OpenSearch (fork of Elasticsearch)
- Kibana (now OpenSearch Dashboards)

---

## ⚙️ How It Works (Architecture Thinking)

1. Data is ingested from:
   - Applications
   - Logs
   - [[Amazon Kinesis Data Firehose]]
   - [[Amazon Kinesis Data Streams]]

2. Data is indexed in OpenSearch cluster

3. Queries/search requests are executed

4. Visualized using OpenSearch Dashboards

👉 OpenSearch = Index + Search + Visualize

---

## 🏗️ Core Components

### 1. Domain (Cluster)
- Collection of nodes (EC2 instances)
- Handles indexing and search

---

### 2. Index
- Logical collection of documents

---

### 3. Document
- JSON data stored in index

---

### 4. Shards
- Data is split into shards
- Enables parallel search

---

## 🧠 Architectural Logic (Why OpenSearch?)

### When to Choose OpenSearch:

✅ Need **full-text search (like Google)**  
✅ Log analytics (ELK stack equivalent)  
✅ Real-time dashboards  
✅ Fast search queries on large datasets  

👉 OpenSearch = Search engine + analytics

---

## ⚖️ OpenSearch vs Other Services (IMPORTANT)

### OpenSearch vs Athena

| Feature | OpenSearch | Athena |
|--------|-----------|--------|
| Use case | Search & logs | Query data |
| Speed | Real-time | Batch query |
| Data type | Indexed JSON | Structured files |

👉 Athena = Query  
👉 OpenSearch = Search  

---

### OpenSearch vs CloudWatch Logs

| Feature | OpenSearch | CloudWatch |
|--------|-----------|------------|
| Analytics | Advanced | Basic |
| Visualization | Rich dashboards | Limited |
| Use case | Large-scale logs | Monitoring |

---

## ⚡ Performance & Scaling

- Scale using:
  - Instance types
  - Number of nodes
  - Shards

👉 More shards = parallel search

---

## 💸 Cost Optimization

- Pay for:
  - Instance usage
  - Storage
  - Data transfer

### Reduce cost:
- Right-size instances
- Use UltraWarm / Cold storage
- Delete old indices (lifecycle policies)

---

## 🔐 Security

- IAM authentication
- Fine-grained access control
- Encryption:
  - At rest (KMS)
  - In transit (HTTPS)
- VPC deployment (private access)

---

## 🔄 Integration with Other Services

- [[Amazon Kinesis Data Firehose]] → ingestion
- [[Amazon Kinesis Data Streams]] → streaming
- [[AWS Lambda]] → transformation
- [[Amazon S3]] → backup storage
- [[Amazon CloudWatch]] → logs

---

## 🚀 Real-World Architecture (Pro Level)

### 📊 Log Analytics System

1. Application logs generated
2. Sent via Firehose
3. Delivered to OpenSearch
4. Indexed and searchable
5. Visualized via dashboards

👉 Real-time monitoring + alerting

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. OpenSearch is NOT for relational queries  
👉 Use [[Amazon RDS]] / [[Amazon Redshift]]

🔥 2. Best for search, not heavy analytics  
👉 Use Athena/Redshift for analytics

🔥 3. Requires indexing  
👉 Data must be structured as documents

🔥 4. Often paired with Firehose  
👉 Common exam pattern

---

## 🧠 Advanced Architect Insight

OpenSearch is used in **observability architecture**:

Logs  
→ Kinesis / Firehose  
→ OpenSearch  
→ Dashboards  

👉 Real-time insights system

---

## 📊 When NOT to Use OpenSearch

❌ Complex SQL queries → Use [[CLP-C02/Amazon Athena]]  
❌ Data warehouse → Use [[Amazon Redshift]]  
❌ Transactional database → Use [[Amazon RDS]]

---

## 🔥 One-Line Summary

👉 OpenSearch = Real-time search and log analytics engine

---

## 🔗 Related Services

- Amazon Kinesis Data Streams
- Amazon Data Firehose
- AWS Lambda
- Amazon S3
- Amazon CloudWatch
- Amazon Athena
- Amazon Redshift