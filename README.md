# 📊 Compliance Data Reconciliation & Risk Validation

## 📌 Project Overview
This project focuses on **reconciling multiple datasets, validating data accuracy, and identifying compliance risks**. It simulates real-world audit and compliance workflows where data inconsistencies can impact decision-making.

The objective is to:
- Ensure **data consistency across datasets**
- Identify **missing and mismatched records**
- Validate data using a **reference dataset**
- Detect **auditor independence risks**
- Generate a **structured compliance report**

---

## 🎯 Key Features
- 🔍 Data Cleaning (missing values, duplicates)
- 🔗 Dataset Reconciliation using joins
- ⚠️ Mismatch Detection
- 🌐 Data Validation using reference dataset
- 🚨 Risk Identification (auditor conflicts)
- 📄 Automated Excel Report Generation

---

## 🗂️ Project Structure

📁 Compliance-Reconciliation-Project
│── 📄 dataset_A.csv
│── 📄 dataset_B.csv
│── 📄 reference_data.csv
│── 📄 compliance_report.xlsx (generated output)
│── 📄 main.ipynb
│── 📄 README.md



---

## 📊 Datasets Description

### 1️⃣ dataset_A.csv
- Primary dataset
- Columns:
  - `company_id`
  - `company_name`
  - `parent_company`
  - `auditor`
- Includes missing values and duplicates

### 2️⃣ dataset_B.csv
- Secondary dataset for comparison
- Contains mismatched company names and extra records

### 3️⃣ reference_data.csv
- Simulates external/public validation source
- Contains verified company records

---

## ⚙️ Step-by-Step Workflow

### 1. Data Loading
- Import datasets using Pandas

### 2. Data Cleaning
- Handle missing values
- Remove duplicates
- Standardize text (lowercase, trim spaces)

### 3. Data Reconciliation
- Merge datasets using `company_id`
- Identify unmatched records

### 4. Inconsistency Detection
- Detect differences in company names across datasets

### 5. Data Validation
- Compare dataset with reference data
- Identify unverified records

### 6. Risk Analysis
- Detect auditor conflicts within the same parent company

### 7. Report Generation
- Export findings into a multi-sheet Excel report

---

## 📈 Output

The project generates:

📄 **compliance_report.xlsx** with the following sheets:

- **Mismatches** → Records missing across datasets  
- **Name Issues** → Company name inconsistencies  
- **Validation Issues** → Unverified records  
- **Risk Cases** → Auditor independence risks  

---

## 💻 Technologies Used
- Python 🐍
- Pandas
- Jupyter Notebook
- Excel (for reporting)

---

