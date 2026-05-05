# 🧠 Amazon Textract

## 🔗 Service Type
#AI #DocumentProcessing #OCR #ML

---

## 📌 What is Amazon Textract?

Amazon Textract is a **fully managed AI service** that:

- Extracts text from documents
- Understands structure (forms, tables)

👉 Textract = “Smart OCR for documents”

---

## ⚙️ How It Works (Architecture Thinking)

1. Input:
   - Scanned documents (PDF, images)
   - Stored in [[Amazon S3]]

2. Textract processes document using ML

3. Outputs:
   - Extracted text
   - Key-value pairs (forms)
   - Tables

👉 Document → Structured data

---

## 🏗️ Key Features (VERY IMPORTANT)

### 1. OCR (Text Extraction)
- Extract raw text

---

### 2. Form Data Extraction
- Key-value pairs:
  - Name → John
  - Date → 01/01/2025

---

### 3. Table Extraction
- Structured table data

---

### 4. Asynchronous Processing
- For large documents

---

## 🧠 Architectural Logic (Why Textract?)

### When to Choose Textract:

✅ Process scanned documents  
✅ Extract structured data  
✅ Automate document workflows  
✅ No ML expertise required  

👉 Textract = Document intelligence

---

## ⚖️ Textract vs Other AI Services (VERY IMPORTANT)

### Textract vs Rekognition

| Feature | Textract | Rekognition |
|--------|----------|-------------|
| Focus | Documents | Images/videos |
| Output | Structured data | Labels/faces |

---

### Textract vs Comprehend

| Feature | Textract | Comprehend |
|--------|----------|------------|
| Input | Documents | Text |
| Output | Extracted data | Insights |

---

## ⚡ Performance & Scaling

- Fully serverless
- Scales automatically

---

## 💸 Cost Optimization

- Pay per:
  - Page processed

### Optimize:
- Process only necessary documents
- Use async mode for large workloads

---

## 🔐 Security

- IAM roles
- Encryption (KMS)
- VPC endpoints

---

## 🔄 Integration with Other Services

- [[Amazon S3]] → document storage
- [[AWS Lambda]] → processing
- [[Amazon Comprehend]] → further analysis
- [[Amazon SNS]] → notifications

---

## 🚀 Real-World Architecture (Pro Level)

### 🧾 Invoice Processing System

1. Upload invoice to S3
2. Lambda triggers Textract
3. Extract:
   - Invoice number
   - Amount
   - Date
4. Store structured data in DB

👉 Automated document processing

---

## ⚠️ Exam Gotchas (VERY IMPORTANT)

🔥 1. Textract ≠ basic OCR  
👉 It extracts structure (tables/forms)

🔥 2. Designed for documents  
👉 Not general images

🔥 3. Works well with Comprehend  
👉 Pipeline pattern

🔥 4. Key keyword:
> “Extract data from forms/tables / document processing”

👉 Answer = Textract

---

## 🧠 Advanced Architect Insight

Textract enables **document automation pipelines**:

S3  
→ Textract  
→ Lambda  
→ Database  

👉 Eliminates manual data entry

---

## 📊 When NOT to Use Textract

❌ General image detection → Use [[Amazon Rekognition]]  
❌ Text analysis → Use [[Amazon Comprehend]]  

---

## 🔥 One-Line Summary

👉 Textract = Extract structured data from documents using AI

---

## 🔗 Related Services

- Amazon S3
- AWS Lambda
- Amazon Comprehend
- Amazon SNS