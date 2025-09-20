# 🛡️ Evidence Chain Management System

<div align="center">

🏛️ **Cryptographically Secure Evidence Management for Legal Professionals**
Ensuring tamper-proof digital evidence with court-admissible chain-of-custody tracking

🚀 Live Demo • 📖 Documentation • 🔧 Installation • 🎯 Features

</div>

---

## 📋 Table of Contents

* 🎯 Overview
* ✨ Key Features
* 🛠️ Technology Stack
* 👥 User Roles & Workflow
* 📊 Example: Complete Website Workflow
* 🚀 Installation & Setup
* 📱 Usage Examples
* 🎨 Screenshots
* 🗺️ Roadmap
* 🤝 Contributing
* 📄 License
* 👤 Author

---

## 🎯 Overview

The **Evidence Chain Management System** is a **secure, web-based platform** built with **Django** for law enforcement agencies, forensic analysts, attorneys, and judges.
It ensures **cryptographic integrity**, **tamper-proof custody tracking**, and **court-admissible documentation**.

---

## ✨ Key Features

* **Cryptographic Security**

  * SHA-256 File Hashing for tamper detection
  * Secure evidence uploads with real-time integrity verification

* **Chain-of-Custody Tracking**

  * Complete audit logs with timestamps & user IDs
  * Digital signatures for every evidence transfer

* **Role-Based Access Control**

  * Detectives → Upload evidence, create cases
  * Forensic Analysts → Analyze evidence, generate reports
  * Attorneys → Review evidence, prepare legal docs
  * Judges → View complete custody trails
  * Admins → Manage users & system settings

* **Court-Ready Documentation**

  * Automated chain-of-custody reports (PDF/Excel)
  * Integrity proofs with digital signatures

---

## 🛠️ Technology Stack

* **Backend**: Django 5.2+, PostgreSQL
* **Security**: hashlib (SHA-256), django-otp (2FA), django-guardian (permissions)
* **Frontend**: Django Templates, Tailwind CSS, **JavaScript** (for interactivity), Chart.js
* **Reports**: ReportLab (PDF), openpyxl (Excel)
* **Deployment**: Docker, Nginx, Gunicorn

---

## 👥 User Roles & Workflow

* **Detective** → Create cases, upload evidence, transfer custody
* **Forensic Analyst** → Verify evidence integrity, conduct analysis, upload reports
* **Attorney** → Review verified evidence, prepare court documentation
* **Judge** → Access complete custody logs and reports
* **System Admin** → Manage roles, security, and server health

---

## 📊 Example: Complete Website Workflow

### 🌐 Evidence Chain Management System

#### 🔐 Step 1: Detective Login & Authentication

* URL: `http://localhost:3000`
* Detective Sharma logs in with **username + password + 2FA**
* Redirected to **dashboard**

#### 🆕 Step 2: Case Creation & Evidence Upload

* Case ID auto-generated → `CC-2025-003`
* Case Title: *Corporate Fraud Investigation*
* Files uploaded:

  * `evidence_001.pdf` → Financial records
  * `suspect_emails.zip` → Email correspondence
  * `financial_records.xlsx` → Spreadsheets
* System generates **SHA-256 hashes** → Integrity verified

#### 🔄 Step 3: Evidence Transfer

* Evidence transferred to **Dr. Priya Singh (Forensic Analyst)**
* Digital signature required → Custody logged

#### 🔬 Step 4: Forensic Analysis

* Analyst verifies file hashes → ✅ No tampering
* Performs metadata & content analysis
* Uploads forensic report → Linked to original evidence

#### 🔍 Step 5: Attorney Review

* Attorney Kumar searches case `CC-2025-003`
* Reviews verified evidence and analysis reports
* Views full **chain-of-custody timeline**

#### 📊 Step 6: Analytics Dashboard

* Live stats:

  * Total Cases: **1,247**
  * Evidence Items: **8,456**
  * Integrity Verification: **100%**
* Charts: Evidence distribution, case completion rates, processing trends

#### 📋 Step 7: Court Report Generation

* Generates **court-ready PDF**:

  * Evidence summary
  * Integrity checks
  * Chain-of-custody timeline
  * Digital signatures

#### ⚙️ Step 8: System Administration

* Admin dashboard shows:

  * Active users (online status)
  * System health & storage usage
  * Backup & uptime logs

---

## 🚀 Installation & Setup

### 📋 Prerequisites

* Python 3.12+
* PostgreSQL 14+
* Redis 7+ (optional for background tasks)

### ⚡ Quick Start

```bash
# 1️⃣ Clone repo
git clone https://github.com/kushagra-sage/Evidence_Chain_System.git
cd evidence-chain-system

# 2️⃣ Create virtual environment
python -m venv .venv
source .venv/bin/activate  # Linux/Mac
.venv\Scripts\activate     # Windows

# 3️⃣ Install dependencies
pip install -r requirements.txt

# 4️⃣ Setup database
python manage.py migrate
python manage.py createsuperuser

# 5️⃣ Start server
python manage.py runserver
```

---

## 📱 Usage Examples

### 🔐 Evidence Upload

```python
POST /evidence/upload/
{
  "case_id": "CC-2025-003",
  "file": "evidence_001.pdf"
}
# System Response
{
  "evidence_id": "CC-2025-003-E001",
  "hash": "a7b8c9d1e2f3...",
  "integrity_verified": true,
  "status": "uploaded"
}
```

### 🔍 Integrity Check

```python
GET /evidence/CC-2025-003-E001/verify/
{
  "status": "VERIFIED",
  "tampered": false
}
```

---

---

## 🗺️ Roadmap

* ✅ Core system (Django + PostgreSQL + Custody tracking)
* 🔄 Advanced reporting (Excel, automated notifications)
* ⏳ Enterprise features (SSO, mobile app, cloud scaling)

---

## 🤝 Contributing

* Follow **PEP 8**
* Maintain **security-first coding**
* Ensure **court admissibility compliance**

---

## 📄 License

MIT License © 2025 \[Kushagra]

---

## 👤 Author

**\[Kushagra]** – Full-Stack Developer & Security Enthusiast

* 🏫 BTech CSE – KIIT University
* 💼 Experience: Django, Security Systems, Full-Stack Dev
* 🔗 GitHub:(https://github.com/kushagra-sage)

---

## 🛡️ Final Note

This system ensures **end-to-end integrity** of digital evidence, providing a **transparent, tamper-proof, and court-ready platform** for the modern justice system.

---
