# 🧠 Amazon QuickSight

## 🔗 Service Type
#Analytics #BI #Visualization #Serverless

---

## 📌 What is Amazon QuickSight?

Amazon QuickSight is a **serverless Business Intelligence (BI) service** used to:

- Visualize data
- Create dashboards
- Generate insights

👉 Think: AWS version of **Power BI / Tableau**

---

## ⚙️ How It Works (Architecture Thinking)

1. Data comes from:
   - [[Amazon S3]]
   - [[CLP-C02/Amazon Athena]]
   - [[Amazon Redshift]]
   - [[Amazon RDS]]

2. QuickSight loads data into:
   - SPICE (in-memory engine)

3. Creates:
   - Dashboards
   - Reports
   - Visualizations

👉 QuickSight = “Last layer of data pipeline (Visualization)”

---

## 🏗️ Core Components

### 1. Data Sources
- Athena, Redshift, S3, RDS

---

### 2. SPICE (VERY IMPORTANT)

- Super-fast in-memory engine
- Improves performance
- Reduces query cost

👉 Key benefit:
- No repeated queries to backend

---

### 3. Dashboards
- Interactive visualizations
- Shareable across users

---

### 4. Datasets
- Prepared data for analysis

---

## 🧠 Architectural Logic (Why QuickSight?)

### When to Choose QuickSight:

✅ Need dashboards & reports  
✅ Business users need insights  
✅ Serverless BI tool required  
✅ Integrated with AWS analytics  

👉 QuickSight = Visualization layer of Data Lake

---

## ⚖️ QuickSight vs Other Services (IMPORTANT)

### QuickSight vs Athena

| Feature | QuickSight | Athena |
|--------|-----------|--------|
| Purpose | Visualization | Query |
| Users | Business users | Engineers |
| Output | Dashboards | Query results |

👉 Athena = Backend  
👉 QuickSight = Frontend  

---

### QuickSight vs OpenSearch

| Feature | QuickSight | OpenSearch |
|--------|-----------|------------|
| Use case | BI dashboards | Log analytics |
| Query type | Structured | Search-based |
| Visualization | Business reports | Technical dashboards |

---

## ⚡ Performance Optimization

### Use SPICE:
- Faster queries
- Lower cost

### Direct Query Mode:
- Real-time data
- Higher cost

👉 Trade-off:
- SPICE = fast + cheap  
- Direct query = real-time  

---

## 💸 Cost Optimization

- Pay for:
  - Users (Authors / Readers)
  - SPICE storage

### Reduce cost:
- Use SPICE
- Limit direct queries
- Optimize dataset size

---

## 🔐 Security

- IAM integration
- Row-level security (RLS)
- Column-level security

👉 Important for multi-user dashboards

---

## 🔄 Integration with Other Services

- [[CLP-C02/Amazon Athena]] → query data
- [[Amazon Redshift]] → warehouse
- [[Amazon S3]] → data lake
- [[AWS Glue]] → ETL
- [[AWS Lake Formation]] → governance

---

## 🚀 Real-World Architecture (Pro Level)

### 📊 Data Lake Analytics Dashboard

1. Data → S3
2. Glue → ETL + catalog
3. Athena → query
4. QuickSight → dashboards

👉 End-to-end serverless analytics system

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. QuickSight is NOT for querying  
👉 Use Athena / Redshift

🔥 2. It is NOT storage  
👉 Uses other services as data source

🔥 3. SPICE is key feature  
👉 Often appears in exam

🔥 4. Key keyword:
> “Dashboard / visualization / BI”

👉 Answer = QuickSight

---

## 🧠 Advanced Architect Insight

QuickSight sits at the **top of analytics architecture**:

S3 (Data Lake)  
→ Glue (ETL)  
→ Athena (Query)  
→ QuickSight (Dashboard)  

---

## 📊 When NOT to Use QuickSight

❌ Need raw data processing → Use [[AWS Glue]]  
❌ Need SQL queries → Use [[CLP-C02/Amazon Athena]]  
❌ Need search analytics → Use [[Amazon OpenSearch Service]]

---

## 🔥 One-Line Summary

👉 QuickSight = Serverless BI tool for dashboards and visualization

---

## 🔗 Related Services

- Amazon Athena
- Amazon Redshift
- Amazon S3
- AWS Glue
- AWS Lake Formation