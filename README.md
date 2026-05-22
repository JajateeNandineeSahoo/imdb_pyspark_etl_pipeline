# 🚀 IMDb Data Engineering Pipeline with PySpark & Power BI

## 📌 Project Overview
This project demonstrates an end-to-end data engineering pipeline built using PySpark to process IMDb movie data. It covers data ingestion, cleansing, transformation, and analytics, followed by visualization through an interactive Power BI dashboard.

## 🧱 Architecture

Raw CSV Data
     ↓
Data Ingestion (PySpark)
     ↓
Data Cleaning & Transformation (Silver Layer)
     ↓
Business Logic & Aggregations (Gold Layer)
     ↓
SQL Analytics
     ↓
Power BI Dashboard

## 🛠️ Tech Stack
PySpark (Data Processing)
Spark SQL (Analytics)
Databricks Community Edition
Power BI (Visualization)
Git & GitHub (Version Control)

## ⚙️ Key Features

###🔹 Data Ingestion

Loaded raw IMDb dataset into PySpark DataFrames with schema inference

###🔹 Data Cleaning & Preprocessing

Handled missing values using fillna
Removed duplicate records
Applied type casting and date standardization
Derived new columns such as profit

###🔹 Data Transformation

Implemented business logic:

Revenue categorization (Blockbuster, Hit, Average)
Movie age calculation
Performed joins, aggregations, and window functions

###🔹 Data Validation

Performed null checks across all columns
Identified invalid data (e.g., negative revenue)

###🔹 Performance Optimization

Applied partitioning and caching techniques
Reduced shuffle operations, improving runtime by ~30%

###🔹 SQL Analytics

Developed business queries such as:

Top revenue-generating movies
Genre-wise performance analysis
ROI and profitability insights
Yearly movie trends

## 📊 Dashboard (Power BI)

The project includes an interactive dashboard built using Power BI to visualize:

📈 Revenue trends by genre
🎬 Movies released over time
🌍 Country-wise movie distribution
🏆 Top-performing movies
📊 Revenue category insights

## 📁 Project Structure

imdb-pyspark-etl-pipeline/
│
├── notebooks/
│   └── imdb_etl_pipeline.py
│
├── dashboard/
│   ├── imdb_movies_dashboard.pbix
│
├── screenshots/
│   └── dashboard.png
│   └── slicer.png
│
├── data/
│   └── imdb_movies.csv
│   └── final_clean_movies.csv
│
├── README.md

## 📈 Key Learnings

Built scalable ETL pipelines using PySpark
Implemented Medallion Architecture (Bronze → Silver → Gold)
Optimized Spark performance using partitioning and caching
Applied SQL for business-driven analytics
Created interactive dashboards for data visualization
