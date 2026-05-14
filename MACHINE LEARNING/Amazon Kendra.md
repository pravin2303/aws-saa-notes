# 🧠 Amazon Kendra

## 🔗 Service Type
#AI #Search #NLP #EnterpriseSearch

---

## 📌 What is Amazon Kendra?

Amazon Kendra is an **intelligent search service** powered by machine learning that allows you to:

- Search across enterprise data sources
- Get accurate, contextual answers
- Use natural language queries

👉 Kendra = “Google-like search for your enterprise data”

---

## ⚙️ How It Works (Architecture Thinking)

1. Connect data sources:
   - [[Amazon S3]]
   - Databases
   - SaaS apps (SharePoint, Salesforce)

2. Kendra indexes content

3. User submits query (natural language)

4. Kendra returns:
   - Relevant results
   - Direct answers

👉 AI-driven search engine

---

## 🏗️ Core Components (VERY IMPORTANT)

### 1. Index
- Stores searchable content

---

### 2. Data Sources
- Connectors for ingesting data

---

### 3. Query Engine
- Processes natural language queries

---

## 🧠 Architectural Logic (Why Kendra?)

### When to Choose Kendra:

✅ Enterprise document search  
✅ Knowledge base systems  
✅ Natural language queries  
✅ Need high relevance results  

👉 Kendra = Intelligent search

---

## ⚖️ Kendra vs Other Services (VERY IMPORTANT)

### Kendra vs OpenSearch

| Feature | Kendra | OpenSearch |
|--------|--------|------------|
| Search type | AI/NLP | Keyword-based |
| Setup | Managed | Requires tuning |
| Accuracy | High | Depends on config |

👉 Kendra = intelligent  
👉 OpenSearch = traditional search  

---

### Kendra vs Comprehend

| Feature | Kendra | Comprehend |
|--------|--------|------------|
| Purpose | Search | Text analysis |
| Output | Results/answers | Insights |

---

## ⚡ Performance & Scaling

- Fully managed
- Scales automatically

---

## 💸 Cost Optimization

- Expensive compared to traditional search

### Use when:
- High-value enterprise search needed

---

## 🔐 Security

- IAM integration
- Access control per document

---

## 🔄 Integration with Other Services

- [[Amazon S3]] → document storage
- [[AWS Lambda]] → processing
- [[Amazon OpenSearch Service]] → alternative search
- [[AWS IAM]] → access control

---

## 🚀 Real-World Architecture (Pro Level)

### 📚 Enterprise Knowledge Base

1. Documents stored in S3
2. Kendra indexes content
3. Employees search using natural language
4. Get direct answers

👉 Improves productivity

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Kendra = search, NOT analytics  
👉 Don’t confuse with Comprehend

🔥 2. Uses ML for relevance  
👉 Key differentiator

🔥 3. Expensive but powerful  
👉 Enterprise use case

🔥 4. Key keyword:
> “Intelligent search / natural language search / enterprise search”

👉 Answer = Kendra

---

## 🧠 Advanced Architect Insight

Kendra enables **AI-powered knowledge discovery**:

Data  
→ Kendra Index  
→ Intelligent Search  

👉 Better than keyword search

---

## 📊 When NOT to Use Kendra

❌ Simple keyword search → Use [[Amazon OpenSearch Service]]  
❌ Text analysis → Use [[Amazon Comprehend]]  

---

## 🔥 One-Line Summary

👉 Kendra = AI-powered enterprise search engine

---

## 🔗 Related Services

- Amazon OpenSearch Service
- Amazon Comprehend
- AWS Lambda
- Amazon S3