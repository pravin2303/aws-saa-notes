# 🧠 AWS Glue

## 🔗 Service Type
#Analytics #ETL #Serverless #DataIntegration

---

## 📌 What is AWS Glue?

AWS Glue is a **serverless ETL (Extract, Transform, Load) service** used to:

- Discover data
- Transform data
- Load data into analytics systems

👉 It eliminates the need to manage ETL infrastructure

---

## ⚙️ How It Works (Architecture Thinking)

1. Data stored in:
   - [[Amazon S3]]
   - Databases (RDS, Redshift, etc.)

2. Glue Crawler scans data
   → Creates metadata in **Glue Data Catalog**

3. Glue ETL Job:
   - Uses Apache Spark
   - Cleans & transforms data

4. Output stored in:
   - S3 (data lake)
   - Redshift (warehouse)

👉 Glue = “Data preparation engine for analytics”

---

## 🏗️ Core Components

### 1. Glue Data Catalog
- Central metadata repository
- Stores:
  - Tables
  - Schema
  - Partitions

👉 Used by:
- [[Amazon Athena]]
- [[Amazon Redshift Spectrum]]
- EMR

---

### 2. Glue Crawler
- Automatically scans data in S3
- Infers schema
- Updates Data Catalog

👉 Removes manual schema definition

---

### 3. Glue ETL Jobs
- Serverless Spark jobs
- Written in:
  - Python (PySpark)
  - Scala

👉 Used for:
- Cleaning data
- Converting formats (CSV → Parquet)

---

### 4. Glue Studio
- Visual interface for ETL pipelines

---

## 🧠 Architectural Logic (Why Glue?)

### When to Choose Glue:

✅ Need ETL pipeline (transform data)  
✅ Data stored in S3 / multiple sources  
✅ Want serverless (no cluster management)  
✅ Need metadata catalog for Athena  

👉 Glue = Backbone of Data Lake

---

## ⚖️ Glue vs EMR vs Athena (VERY IMPORTANT)

| Service | Purpose |
|--------|--------|
| [[AWS Glue]] | ETL (transform data) |
| [[Amazon EMR]] | Complex big data processing |
| [[Amazon Athena]] | Query data |

👉 Simple rule:
- Glue → Prepare data  
- EMR → Heavy processing  
- Athena → Query data  

---

## ⚡ Performance Optimization

### 1. Use Partitioning
- Improves query performance

### 2. Convert to Columnar Format
- Parquet / ORC → faster queries

### 3. Use Job Bookmarks
- Process only new data

---

## 💸 Cost Optimization

- Pay per:
  - Data Processing Units (DPUs)
  - Job execution time

### Reduce cost:
- Use job bookmarks (avoid reprocessing)
- Optimize transformations
- Use Glue version 3+ (better performance)

---

## 🔐 Security

- IAM roles for access
- Encryption:
  - Data at rest (S3/KMS)
  - In transit (TLS)
- Fine-grained access via [[AWS Lake Formation]]

---

## 🔄 Integration with Other Services

- [[Amazon S3]] → Data Lake
- [[Amazon Athena]] → Query
- [[Amazon Redshift]] → Data warehouse
- [[Amazon EMR]] → Advanced processing
- [[AWS Lake Formation]] → Governance

---

## 🚀 Real-World Architecture (Pro Level)

### 📊 Data Lake Pipeline

1. Raw data → S3
2. Glue Crawler → create schema
3. Glue Job → clean & convert data
4. Store processed data in S3 (Parquet)
5. Query using Athena
6. Visualize using QuickSight

👉 Fully serverless pipeline

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Glue is NOT for querying  
👉 Use Athena for queries

🔥 2. Glue is NOT for real-time streaming  
👉 Use Kinesis

🔥 3. Glue = serverless ETL  
👉 No EC2 cluster (unlike EMR)

🔥 4. Glue Data Catalog is KEY  
👉 Many services depend on it

---

## 🧠 Advanced Architect Insight

Glue is the **bridge between raw data and analytics**:

S3 (Raw Data)  
→ Glue (ETL + Catalog)  
→ Athena / Redshift (Query)  

---

## 📊 When NOT to Use Glue

❌ Simple queries → Use [[Amazon Athena]]  
❌ Heavy custom processing → Use [[Amazon EMR]]  
❌ Real-time streaming → Use [[Amazon Kinesis]]

---

## 🔥 One-Line Summary

👉 Glue = Serverless ETL + Data Catalog for data lake architecture

---

## 🔗 Related Services

- Amazon S3
- Amazon Athena
- Amazon EMR
- Amazon Redshift
- AWS Lake Formation

## Mini Memory Trick

- Glue = Prepare data 🧹
- Athena = Query data 🔍
- EMR = Process data 🏗️