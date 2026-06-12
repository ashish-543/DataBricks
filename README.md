# 🚀 Databricks Data Engineering Repository

A collection of Data Engineering projects built using **PySpark**, **Databricks**, **Delta Lake**, and **Structured Streaming**. This repository covers data ingestion, transformation, modeling, enrichment, and real-time processing.

## 📂 Repository Structure

### 🌐 API Integration

Enriches incomplete CSV data using a REST API.

**Workflow:**

* Read source CSV file
* Extract `user_id`
* Fetch data from REST API based on the user_id
* Flatten JSON responses
* Select required fields
* Merge API data with CSV data to create an enriched dataset

**Concepts:** REST APIs, JSON Flattening, Data Enrichment, Joins

---

### 🏗️ Data Modeling

Implements a Medallion Architecture (Bronze → Silver → Gold).

* **🥉 Bronze:** Incremental data loading using `order_date > last_load_date`
* **🥈 Silver:** Data cleansing, transformations, and upserts using `MERGE`
* **🥇 Gold:** Star Schema implementation with Fact and Dimension tables
* **🔄 SCD:** Type 1 and Type 2 Slowly Changing Dimensions

**Concepts:** Delta Lake, Incremental Loading, Star Schema, SCD, Data Warehousing

---

### ⚡ PySpark

Collection of commonly used PySpark transformation functions and UDFs.

**Includes:**

* DataFrame Transformations
* Joins
* Aggregations
* Window Functions
* UDFs
* Schema Operations

---

### 📡 Spark Streaming

Real-time data processing using PySpark Structured Streaming.

**Features:**

* Continuous Data Ingestion
* Streaming Transformations
* Checkpointing
* Fault Tolerance

---

## 🛠️ Technologies

* Python
* PySpark
* Databricks
* Delta Lake
* SQL
* REST APIs
* Apache Spark Structured Streaming

---

## 🎯 Key Learning Areas

- ✅ API Data Extraction & Enrichment
- ✅ Incremental ETL Pipelines
- ✅ Medallion Architecture
- ✅ Star Schema Modeling
- ✅ SCD Type 1 & Type 2
- ✅ PySpark Transformations
- ✅ Real-Time Data Processing

# 👨‍💻 Author

**Ashish Pandeya**

- Data Engineering | PySpark | Databricks | Delta Lake | Apache Spark

---

## ⭐ If you found this project useful, consider giving it a star!
