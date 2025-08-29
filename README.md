# 🧾 Serverless Receipt Automation on AWS

**Automating receipt organization: no servers, just speed and scale!**

This project simplifies how receipts and invoices are processed and organized—entirely using serverless and managed AWS services. Simply upload a document, and a clean summary will be delivered straight to your inbox.

---

## 🚀 How It Works

📤 **Upload a Receipt or Invoice** to an S3 bucket  
⚙️ **Lambda Function** automatically processes the document  
🧾 **Textract** extracts relevant text and data  
📦 **DynamoDB** stores the structured output  
📨 **SES** sends a formatted summary via email

All with **no servers**, minimal cost, and built-in scalability.

---

## 🧱 Architecture Overview

This project follows AWS Well-Architected Framework principles, focusing on scalability, fault tolerance, cost-efficiency, and security.

| Component         | Purpose                                              |
|------------------|------------------------------------------------------|
| **Amazon S3**     | Stores uploaded receipts and invoices                |
| **AWS Lambda**    | Orchestrates the processing flow                     |
| **Amazon Textract** | Extracts key text and structured data              |
| **Amazon DynamoDB** | Persists processed data for later retrieval        |
| **Amazon SES**     | Sends email with the summarized result              |
| **AWS IAM**        | Manages roles and permissions securely              |

---

## 🧠 Lambda Function Responsibilities

The Lambda function is the core of the automation:

- 🎯 **Handler Logic** – Triggers when new documents arrive in S3
- 🔍 **Textract Integration** – Extracts important fields from receipts
- 🧱 **Database Layer** – Saves parsed data to DynamoDB
- 📬 **Email Sender** – Sends the summary email via SES

---

## 📈 Use Cases

This solution is ideal for:

- ✅ E-commerce platforms organizing digital invoices  
- ✅ Freelancers tracking receipts for tax season  
- ✅ Finance/admin teams managing daily expen
