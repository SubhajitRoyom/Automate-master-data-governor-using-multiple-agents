
# Automated Master Data Governor using Multi-Agent AI

## 🚀 Overview

This project is an end-to-end data quality automation system built using **n8n, AI Agents, and SQL execution pipelines**.
It identifies data issues, fixes them using SQL, and generates a professional report automatically.

---

## 🧠 Problem Statement

Organizations struggle with:

* Missing or inconsistent data
* Duplicate records
* Invalid formats (emails, dates, phone numbers)
* Lack of governance on data quality

This project automates:
✔ Detection
✔ Fixing
✔ Reporting

---

## ⚙️ Architecture

The system consists of **three AI agents**:

### 1. Data Investigator Agent

* Scans database
* Identifies issues
* Outputs structured JSON

### 2. Data Issue Fixer Agent

* Generates SQL queries
* Executes fixes in PostgreSQL
* Returns execution results

### 3. Data Investigation Reporter Agent

* Generates a **Database Health Check Report**
* Creates Google Docs report
* Shares public link

---

## 🔄 Workflow (n8n)

1. Investigate database issues
2. Send for approval (manual checkpoint)
3. Fix issues using SQL
4. Aggregate results
5. Generate report
6. Share report via Google Drive

---

## 📦 Tech Stack

* n8n (workflow automation)
* Google Gemini (AI Agent)
* PostgreSQL (database)
* Google Docs API
* Google Drive API

---

## 📁 Key Components

### Workflows

* `workflows/n8n-workflow.json` → main automation flow


### Schemas

* `schemas/sql_output_schema.json`
* `schemas/report_output_schema.json`

---

## 📊 Sample Output

### Report Includes:

* Executive Summary
* Fixed Issues
* Discussion Items
* Not Fixed Issues

---

## 🧪 How to Run

1. Import workflow into n8n
2. Configure:

   * Google Docs credentials
   * Google Drive credentials
   * PostgreSQL connection
3. Execute workflow

---

## 🎯 Use Cases

* Data governance automation
* Data quality monitoring
* Enterprise reporting automation

---

## 💡 Future Improvements

* Add real-time monitoring
* Integrate with BI tools (Power BI, Tableau)
* Add alerting system

---

## 👤 

Subhajit Roy
