# 🧠 AWS Wavelength

## 🔗 Service Type
#Compute #EdgeComputing #LowLatency #5G

---

## 📌 What is AWS Wavelength?

AWS Wavelength is a service that brings AWS compute and storage **closer to mobile users** by embedding AWS infrastructure inside **5G telecom networks**.

👉 Wavelength = “AWS at the edge of 5G networks”

---

## ⚙️ How It Works (Architecture Thinking)

1. AWS deploys infrastructure in telecom provider data centers

2. Applications run on:
   - [[Amazon EC2]]
   - [[Amazon EBS]]

3. Mobile users connect via 5G network

4. Requests handled locally (low latency)

👉 No need to route traffic to AWS Region

---

## 🏗️ Core Components

### 1. Wavelength Zone
- Extension of a VPC
- Located inside telecom network

---

### 2. Carrier Gateway
- Connects mobile devices to AWS workloads

---

### 3. EC2 Instances
- Run applications close to users

---

## 🧠 Architectural Logic (Why Wavelength?)

### When to Choose Wavelength:

✅ Ultra-low latency required (single-digit ms)  
✅ Mobile applications (5G users)  
✅ Real-time apps:
   - Gaming
   - AR/VR
   - Video streaming  

👉 Wavelength = Mobile edge computing

---

## ⚖️ Wavelength vs Other Edge Options (VERY IMPORTANT)

### Wavelength vs Local Zones

| Feature | Wavelength | Local Zones |
|--------|-----------|-------------|
| Location | Telecom network | AWS city locations |
| Latency | Ultra-low (5G) | Low |
| Use case | Mobile apps | General apps |

---

### Wavelength vs CloudFront

| Feature | Wavelength | CloudFront |
|--------|-----------|------------|
| Purpose | Compute at edge | Content delivery |
| Use case | Real-time processing | Caching content |

---

### Wavelength vs Outposts

| Feature | Wavelength | Outposts |
|--------|-----------|----------|
| Location | Telecom edge | On-prem |
| Use case | Mobile users | Local data center |

---

## ⚡ Performance & Latency

- Single-digit millisecond latency
- Optimized for mobile traffic

---

## 💸 Cost Optimization

- Pay for:
  - EC2 usage
  - Data transfer

👉 Use only when low latency is critical

---

## 🔐 Security

- Same AWS security model:
  - IAM
  - VPC isolation
- Telecom network security integration

---

## 🔄 Integration with Other Services

- [[Amazon EC2]] → compute
- [[Amazon EBS]] → storage
- [[Amazon VPC]] → networking
- AWS Region → backend processing

---

## 🚀 Real-World Architecture (Pro Level)

### 🎮 Mobile Gaming Platform

1. Game servers deployed in Wavelength Zone
2. Players connect via 5G
3. Real-time gameplay with ultra-low latency
4. Backend data stored in AWS Region

👉 High-performance mobile experience

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Wavelength = mobile edge  
👉 Not general edge

🔥 2. Requires 5G network  
👉 Key requirement

🔥 3. Ultra-low latency  
👉 Main use case

🔥 4. Key keyword:
> “5G / mobile users / ultra-low latency”

👉 Answer = Wavelength

---

## 🧠 Advanced Architect Insight

Wavelength enables **edge architecture for mobile apps**:

Mobile Device  
→ Wavelength Zone  
→ AWS Region  

👉 Split processing (edge + cloud)

---

## 📊 When NOT to Use Wavelength

❌ General applications → Use [[AWS Local Zones]]  
❌ Content delivery → Use [[Amazon CloudFront]]  
❌ On-prem workloads → Use [[AWS Outposts]]  

---

## 🔥 One-Line Summary

👉 AWS Wavelength = Run applications at the edge of 5G networks for ultra-low latency

---

## 🔗 Related Services

- Amazon EC2
- Amazon EBS
- Amazon VPC
- AWS Local Zones
- AWS Outposts
- Amazon CloudFront

# 🔥 Edge Computing Mental Model

- CloudFront → Cache content 🌍
- Local Zones → Near users 🏙️
- Wavelength → 5G edge 📡
- Outposts → On-prem 🏢