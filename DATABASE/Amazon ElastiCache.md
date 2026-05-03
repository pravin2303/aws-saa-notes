# 🧠 Amazon ElastiCache

## 🔗 Service Type
#Database #Caching #InMemory #Performance

---

## 📌 What is Amazon ElastiCache?

Amazon ElastiCache is a **fully managed in-memory caching service** used to:

- Cache frequently accessed data
- Reduce database load
- Improve application performance

👉 ElastiCache = “RAM-based database for speed”

---

## ⚙️ How It Works (Architecture Thinking)

1. Application queries cache first

2. If cache hit:
   - Return data instantly

3. If cache miss:
   - Fetch from DB
   - Store in cache

👉 Cache layer sits between app and database

---

## 🏗️ Supported Engines (VERY IMPORTANT)

### 1. Redis

- Advanced features:
  - Persistence
  - Replication
  - Pub/Sub
- Multi-AZ support

👉 Most commonly used

---

### 2. Memcached

- Simple key-value cache
- No persistence
- Multi-threaded

👉 High-speed caching only

---

## 🧠 Architectural Logic (Why ElastiCache?)

### When to Choose ElastiCache:

✅ Reduce database load  
✅ Improve latency (microseconds)  
✅ Handle read-heavy workloads  
✅ Session management  

👉 ElastiCache = Performance booster

---

## ⚖️ Redis vs Memcached (VERY IMPORTANT)

| Feature | Redis | Memcached |
|--------|------|-----------|
| Persistence | Yes | No |
| Replication | Yes | No |
| Multi-thread | No | Yes |
| Features | Advanced | Simple |

👉 Redis = most use cases  
👉 Memcached = simple caching  

---

## ⚡ Performance & Scaling

- In-memory → ultra-fast
- Scale via:
  - Clustering
  - Sharding (Redis)

---

## 💸 Cost Optimization

- Reduces DB cost by:
  - Lower read load
  - Fewer queries

### Optimize:
- Cache only frequently accessed data
- Use TTL (expiration)

---

## 🔐 Security

- VPC isolation
- Encryption:
  - At rest
  - In transit
- IAM (limited support)

---

## 🔄 Integration with Other Services

- [[Amazon EC2]] → application
- [[Amazon RDS]] → primary DB
- [[Amazon DynamoDB]] → caching layer
- [[AWS Lambda]] → serverless apps

---

## 🚀 Real-World Architecture (Pro Level)

### 🌐 High-Traffic Web App

1. User request → app server
2. Check Redis cache
3. If miss → query DB (RDS/Aurora)
4. Store result in cache

👉 Reduces DB load + improves speed

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. ElastiCache = NOT primary database  
👉 It is a cache layer

🔥 2. Redis supports persistence  
👉 Memcached does NOT

🔥 3. Used for read-heavy workloads  
👉 Key pattern

🔥 4. Key keyword:
> “Improve performance / reduce DB load / caching”

👉 Answer = ElastiCache

---

## 🧠 Advanced Architect Insight

ElastiCache enables **high-performance architecture**:

App  
→ Cache (Redis)  
→ Database  

👉 Minimizes DB bottleneck

---

## 📊 When NOT to Use ElastiCache

❌ As primary database → Use [[Amazon RDS]] / [[Amazon DynamoDB]]  
❌ Write-heavy workloads  

---

## 🔥 One-Line Summary

👉 ElastiCache = In-memory cache to improve performance and reduce database load

---

## 🔗 Related Services

- Amazon RDS
- Amazon Aurora
- Amazon DynamoDB
- Amazon EC2
- AWS Lambda