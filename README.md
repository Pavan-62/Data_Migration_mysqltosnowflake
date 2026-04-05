# End-to-End Data Pipeline: On-Premise MySQL to Snowflake using Azure Data Factory

## 📌 Overview
This project demonstrates an end-to-end ELT pipeline to migrate data from an on-premise MySQL database to Snowflake using Azure Data Factory (ADF). Azure Blob Storage is used as a staging layer due to limitations in direct data transfer.

---

## 🏗️ Architecture
On-Premise MySQL → ADF (Self-Hosted Integration Runtime) → Azure Blob Storage (Staging) → Snowflake

---

## ⚙️ Key Components

### 🔹 Azure Data Factory
- Orchestrates the data pipeline
- Uses Copy Activity for data movement
- Supports scheduling via triggers

### 🔹 Self-Hosted Integration Runtime
- Enables secure connection to on-premise MySQL
- Installed locally to bridge on-prem and cloud systems

### 🔹 Azure Blob Storage (Staging)
- Acts as an intermediate storage layer
- Required for transferring data from MySQL to Snowflake

### 🔹 Snowflake
- Cloud data warehouse used as final destination
- Stores structured data for analytics

---

## 🔄 Pipeline Workflow

1. Extract data from on-premise MySQL database  
2. Transfer data to Azure Blob Storage (staging layer)  
3. Load data from staging into Snowflake  
4. Perform schema mapping between source and target  
5. Trigger and monitor pipeline execution  

---

## 🛠️ Implementation Steps

- Configured Self-Hosted Integration Runtime for on-prem connectivity  
- Created Linked Services for MySQL, Azure Blob Storage, and Snowflake  
- Built pipeline using Copy Activity  
- Enabled staging using Azure Blob Storage  
- Automated execution using triggers  
- Monitored execution using ADF Monitor  

---

## 🧠 Concepts Used
- ELT Pipeline Design  
- Data Migration  
- Pipeline Orchestration  
- Cloud Data Warehousing  
- Staging Layer Architecture  

---

## 🚀 Key Learnings
- Built and orchestrated data pipelines using Azure Data Factory  
- Understood integration between on-premise and cloud systems  
- Learned staging-based data migration strategy  
- Gained experience in Snowflake data loading  

---

## 📎 Note
This project was implemented for learning purposes and demonstrates core data engineering concepts using Azure Data Factory and Snowflake.
