# 🛡️ Vigilant.AI  
### Pre-Disbursement Early Warning Engine for Multi-Tier Supply Chain Fraud  

**IntelliTrace Hackathon 2026 Submission**  
**Problem Statement:** Multi-Tier Supply Chain Fraud Detection  
**Team:** Team 007 | VIT Bhopal University  

---

## 📖 Project Overview

Vigilant.AI is a real-time fraud detection system designed to prevent multi-tier supply chain financing fraud, specifically targeting **phantom invoicing** and **cross-tier cascading exposure**.

In traditional supply chain finance (Tier 1 → Tier 2 → Tier 3), banks evaluate invoices in isolation. This creates visibility blind spots, enabling fraudsters to submit forged invoices to multiple lenders simultaneously.

Vigilant.AI shifts fraud detection from reactive post-audit recovery to **proactive, pre-disbursement prevention** by generating a dynamic **Fraud Risk Score** before capital is released.

---

## 🚀 Core Technical Architecture

### 1️⃣ 3-Way Data Triangulation (Zero-Trust Validation)

Instead of trusting the invoice alone, the system cross-validates:

- **Corporate ERP Data**  
  - Purchase Orders (PO)  
  - Goods Receipt Notes (GRN)  

- **Government GST Records**  
  - Tax filing consistency  
  - Invoice value verification  

- **Core Banking Ledger**  
  - Historical transaction behavior  
  - Fund flow validation  

✅ Result: Instantly flags fake billing, inflated invoices, and physically impossible phantom transactions.

---

### 2️⃣ Graph Network Intelligence

Using **NetworkX**, we model:

- Companies → Nodes  
- Financial transactions → Edges  

This enables detection of:

- Circular Trading Loops  
- Cascading Exposure Patterns  
- Suspicious Supply Chain Topologies  

Traditional SQL queries cannot detect these network-level anomalies.

---

### 3️⃣ Machine Learning & NLP Defense Layer

#### 🔹 Isolation Forest (Unsupervised Anomaly Detection)
- Detects abnormal invoice submission velocity  
- Flags extreme invoice amount outliers  
- Works without perfectly labeled fraud datasets  

#### 🔹 NLP Smart Fingerprinting (Cosine Similarity)
- Detects near-duplicate invoices  
- Identifies minor text alterations used to bypass MD5 hash checks  
- Prevents cross-lender duplicate financing  

---

## 🛠️ Proposed Tech Stack

### Backend
- Python  
- REST API Handling  
- Real-Time Data Processing  

### Machine Learning
- Scikit-Learn (Isolation Forest)  
- NetworkX (Graph Analytics)  
- NLTK / TF-IDF (Cosine Similarity)  

### Database
- MySQL  
- Relational linking of ERP, GST, and Banking datasets  

### Frontend
- HTML  
- CSS  
- JavaScript  
- Compliance Dashboard for Risk Visualization  

---

## ⚙️ System Workflow

1. Invoice Submitted  
2. 3-Way Data Triangulation  
3. Feature Extraction (Velocity, Feasibility, Sequencing)  
4. Graph Analysis  
5. ML Risk Scoring  
6. Fraud Risk Score Generated  
7. Approve / Block Disbursement  

---

## 📊 Key Features

- Pre-Disbursement Fraud Prevention  
- Real-Time Risk Scoring  
- Graph-Based Exposure Mapping  
- Duplicate Invoice Detection  
- Zero-Trust Validation Architecture  
- NPA Risk Mitigation  

---

## 🎯 Business Impact

- Prevents multi-million dollar exposure before disbursement  
- Reduces creation of Non-Performing Assets (NPAs)  
- Enhances KYB (Know Your Business) visibility  
- Automates PO–GRN–GST validation  
- Strengthens compliance intelligence  

---

## 🔮 Future Roadmap

- Direct GSTN API Integration  
- RBI Account Aggregator Integration  
- Inter-Bank Encrypted Invoice Hash Ledger  
- Scalable Cloud Deployment  

---

## 👥 Team Details

**Team Name:** Team 007  
**Institution:** VIT Bhopal University  

**Members:**
- Rishav Raj (Team Leader)  
- Perepu Soumya  
- Tejaswani Yadav  
- Lokesh Kewat  

---

## 📌 Conclusion

Vigilant.AI transforms fraud detection in supply chain finance from reactive recovery into a proactive, algorithm-driven capital protection system.

By combining 3-Way Data Triangulation, Graph Intelligence, and Machine Learning, we build a real-time defense layer that protects banks before capital loss occurs.
