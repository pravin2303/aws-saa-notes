# 🧠 Amazon Kinesis

## 🔗 Service Type
#Analytics #Streaming #RealTime #DataIngestion

---

## 📌 What is Amazon Kinesis?

Amazon Kinesis is a **real-time data streaming platform** that enables you to:

- Collect
- Process
- Analyze streaming data

👉 Handles continuous data like:
- Logs
- Clickstreams
- IoT data
- Metrics

---

## 🏗️ Kinesis Family (VERY IMPORTANT)

### 1. Kinesis Data Streams (KDS)
- Real-time streaming (low latency)
- Full control over consumers

### 2. Kinesis Data Firehose
- Serverless delivery (near real-time)
- No management required

### 3. Kinesis Data Analytics
- Real-time SQL / Apache Flink processing

### 4. Kinesis Video Streams
- Video streaming ingestion

---

## ⚙️ Kinesis Data Streams (Core Service)

### How It Works:

1. Producers send data to stream
2. Data stored in **shards**
3. Consumers read data:
   - EC2 apps
   - Lambda
   - Analytics services

👉 Data retained for:
- 24 hours (default)
- Up to 365 days

---

## 🧠 Key Concept: Shards

- Each shard provides:
  - 1 MB/s write
  - 2 MB/s read

👉 More shards = more throughput

---

## 🏗️ Architectural Logic (Why Kinesis?)

### When to Choose Kinesis:

✅ Need **real-time (<1 sec) processing**  
✅ Need **multiple consumers**  
✅ Need **data replay capability**  
✅ Need **fine-grained control**

👉 Kinesis = High-control streaming system

---

## ⚖️ Kinesis vs Firehose (VERY IMPORTANT)

| Feature | Kinesis Data Streams | Firehose |
|--------|---------------------|----------|
| Latency | Real-time | Near real-time |
| Control | Full | Limited |
| Replay | ✅ Yes | ❌ No |
| Management | Required | Fully managed |
| Use case | Complex processing | Simple delivery |

👉 Exam shortcut:
- Complex → Kinesis Streams  
- Simple → Firehose  

---

## ⚡ Performance & Scaling

- Scale using **shards**
- Supports:
  - Parallel processing
  - High throughput ingestion

👉 Auto scaling available (on-demand mode)

---

## 💸 Cost Optimization

- Pay per:
  - Shard usage
  - Data ingestion
  - Data retention

### Reduce cost:
- Use on-demand mode
- Optimize shard count
- Reduce retention period

---

## 🔐 Security

- IAM for access control
- Encryption:
  - At rest (KMS)
  - In transit (HTTPS)

---

## 🔄 Integration with Other Services

- [[AWS Lambda]] → real-time processing
- [[Amazon S3]] → storage
- [[Amazon Redshift]] → analytics
- [[Amazon OpenSearch Service]] → search
- [[AWS Glue]] → ETL

---

## 🚀 Real-World Architecture (Pro Level)

### 📊 Real-Time Analytics Pipeline

1. Users generate clickstream data
2. Data sent to Kinesis Data Streams
3. Lambda processes data in real time
4. Store results in:
   - S3 (data lake)
   - OpenSearch (dashboard)

👉 Real-time insights (sub-second latency)

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Kinesis = real-time (<1 sec)  
👉 Firehose = near real-time (buffered)

🔥 2. Kinesis supports replay  
👉 Firehose does NOT

🔥 3. Kinesis requires shard management  
👉 Firehose does NOT

🔥 4. Multiple consumers supported  
👉 Important for analytics pipelines

---

## 🧠 Advanced Architect Insight

Kinesis enables **event-driven architecture**:

Producers  
→ Kinesis Streams  
→ Multiple Consumers (Lambda, apps)  
→ Storage / Analytics  

👉 Decoupled, scalable system

---

## 📊 When NOT to Use Kinesis

❌ Simple ingestion → Use [[Amazon Data Firehose]]  
❌ Batch processing → Use [[Amazon EMR]]  
❌ Ad-hoc queries → Use [[Amazon Athena]]  

---

## 🔥 One-Line Summary

👉 Kinesis = Real-time streaming platform with high control and scalability

---

## 🔗 Related Services

- Amazon Data Firehose
- AWS Lambda
- Amazon S3
- Amazon Redshift
- Amazon OpenSearch Service
- AWS Glue