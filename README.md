# 🛍️ Deal_Watch - Cloud-Based Discount & Promotion Detection

## 📖 Overview
**DealWatch** is a cloud-based data engineering project designed to collect, process, and analyze product prices and promotions from multiple e-commerce websites.  
The system detects discounts and price drops automatically, stores the data in a data lake, and visualizes real-time insights in a dashboard.

This project demonstrates **end-to-end Data Engineering skills** — from data ingestion and transformation to cloud orchestration and visualization.

---

## 🏗️ Architecture
The pipeline follows a **Data Lake + Orchestration** architecture using AWS and Python:

1. **Ingestion (Raw Zone)** – Web scrapers and API collectors fetch product data and store it in **Amazon S3 (raw)**.  
2. **Transformation (Silver Zone)** – Data is cleaned, normalized, and enriched using **AWS Glue / Pandas / PySpark**.  
3. **Analytics (Gold Zone)** – Aggregated price trends and discount flags are stored in **Athena** or **Redshift** for querying.  
4. **Visualization** – A **Streamlit dashboard** displays price history, top daily discounts, and category trends.  
5. **Automation** – **Airflow (MWAA)** or **EventBridge + Lambda** orchestrate daily ingestion and transformations.

