# Local AI-Powered Compliance Audit Engine 🤖🏦

## 🎯 Project Overview
This project demonstrates a "Privacy-First" approach to automated banking audits. It uses a local Large Language Model (Llama 3.1) to interpret unstructured PDF policies and cross-reference them against structured customer data in Excel.

## 🌟 Why This Matters (The "Audit" Angle)
In traditional banking environments, uploading sensitive PII (Personally Identifiable Information) to cloud-based AI like ChatGPT is a major security risk. This solution solves that by using **Local Inference**:
- **Data Residency:** All data stays on the local machine.
- **Cost-Effective:** Zero API costs; uses open-source models via Ollama.
- **Scalable:** Can be adjusted to read any PDF policy and audit any Excel dataset.

## 🛠️ The Tech Stack
- **Language:** Python 3.12 (Environment managed via Conda)
- **AI Engine:** Ollama (Llama 3.1) 
- **Key Libraries:** Pandas (Data), PDFPlumber (Text Extraction), OpenPyXL (Excel)

## 🚀 How It Works
1. **Rule Extraction:** The script feeds a PDF policy to Llama 3.1 and asks it to determine mandatory vs. optional document requirements.
2. **Automated Cross-Check:** The Python engine scans the customer spreadsheet to see if those mandatory requirements are met.
3. **Exception Reporting:** An automated Excel report is generated, highlighting only the customers who are out of compliance for immediate remediation.

---
*Developed as a proof-of-concept for modernizing compliance workflows through local AI automation.*

