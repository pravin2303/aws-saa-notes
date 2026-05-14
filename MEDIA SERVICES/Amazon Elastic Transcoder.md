# 🧠 Amazon Elastic Transcoder

## 🔗 Service Type
#Media #VideoProcessing #Transcoding #Streaming

---

## 📌 What is Amazon Elastic Transcoder?

Amazon Elastic Transcoder is a service that:

- Converts media files (video/audio)
- Into different formats for playback on devices

👉 Transcoder = “Convert video formats for different devices”

---

## ⚙️ How It Works (Architecture Thinking)

1. Upload media file to [[Amazon S3]]

2. Elastic Transcoder processes file

3. Outputs converted files to S3

👉 Input → Convert → Output

---

## 🏗️ Core Components (VERY IMPORTANT)

### 1. Pipeline

- Workflow configuration

---

### 2. Job

- Conversion task

---

### 3. Presets

- Predefined encoding settings

---

## 🧠 Architectural Logic (Why Elastic Transcoder?)

### When to Choose Elastic Transcoder:

✅ Basic video transcoding  
✅ Simple media workflows  
✅ Multi-device compatibility  

👉 Transcoder = Media format conversion

---

## ⚖️ Elastic Transcoder vs MediaConvert (VERY IMPORTANT)

| Feature | Elastic Transcoder | MediaConvert |
|--------|------------------|--------------|
| Status | Legacy | Modern |
| Features | Basic | Advanced |
| Use case | Simple conversion | Professional workflows |

👉 MediaConvert = preferred  
👉 Transcoder = basic  

---

## ⚡ Key Features (IMPORTANT)

### 1. Multiple Output Formats
- Mobile, web, TV

---

### 2. Integration with S3
- Storage + processing

---

### 3. Managed Service
- No infrastructure required

---

## ⚡ Performance & Scaling

- Automatically scales

---

## 💸 Cost Optimization

- Pay per:
  - Minutes of video processed

---

## 🔐 Security

- IAM roles
- S3 access control

---

## 🔄 Integration with Other Services

- [[Amazon S3]] → input/output storage
- [[AWS Lambda]] → trigger jobs
- [[Amazon CloudWatch]] → monitoring

---

## 🚀 Real-World Architecture (Pro Level)

### 🎬 Video Streaming Pipeline

Upload video → S3  
→ Transcoder  
→ Output formats (mobile, web)  
→ CDN delivery  

👉 Multi-device streaming

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Elastic Transcoder = video conversion ONLY  
👉 Not streaming

🔥 2. Legacy service  
👉 Prefer MediaConvert

🔥 3. Uses S3 for storage  
👉 Key integration

🔥 4. Key keyword:
> “Convert video formats / transcoding”

👉 Answer = Elastic Transcoder

---

## 🧠 Advanced Architect Insight

Modern architecture:

S3  
→ MediaConvert (preferred)  
→ CloudFront  

👉 Scalable media pipeline

---

## 📊 When NOT to Use Elastic Transcoder

❌ Advanced workflows → Use [[AWS Elemental MediaConvert]]  
❌ Real-time streaming → Use MediaLive  

---

## 🔥 One-Line Summary

👉 Elastic Transcoder = Basic service to convert media files into different formats

---

## 🔗 Related Services

- AWS Elemental MediaConvert
- Amazon S3
- Amazon CloudFront