# 🛒 Retail Customer Analytics, Churn Intelligence & Automation System

## 📌 Project Overview

This project is an end-to-end Retail Customer Intelligence System that combines:

* Data Analytics
* Customer Segmentation (RFM)
* Churn Risk Detection
* Machine Learning Prediction
* Revenue-at-Risk Analysis
* Action Recommendation Engine
* SQL Data Warehouse Integration
* Power BI Business Dashboard
* Automated Data Pipeline

The goal is to help retail businesses reduce churn, protect revenue, and prioritize customer retention using data-driven intelligence.

---

# 🎯 Business Problem

Retail companies struggle with:

* Identifying high-value customers
* Detecting early churn signals
* Prioritizing retention efforts
* Understanding revenue risk exposure
* Making explainable ML-based decisions

This system solves those problems using structured analytics and predictive modeling.

---

# 🏗️ System Architecture

```
Raw Retail Data
        ↓
Data Cleaning (Python)
        ↓
RFM Analysis
        ↓
Churn Intelligence Engine
        ↓
Machine Learning Model
        ↓
Customer Priority Scoring
        ↓
MySQL Data Warehouse
        ↓
Power BI Dashboard
        ↓
Automated Decision & Action Recommendations
```

---

# 🗂️ Data Source

Retail transaction dataset containing:

* Invoice Number
* Product Description
* Customer ID
* Invoice Date
* Quantity
* Unit Price
* Country

Data is cleaned, transformed, and stored in MySQL for structured analytics.

---

# ⚙️ Project Workflow

---

## 1️⃣ Data Cleaning & Preparation (Python)

* Removed negative quantity records
* Removed cancelled invoices
* Handled missing customer IDs
* Created `Total_Amount = Quantity × Unit Price`
* Converted date columns
* Created monthly and time-based features

Libraries used:

* pandas
* numpy

---

## 2️⃣ SQL Data Warehouse Integration

* Stored cleaned data in MySQL
* Created customer-level analytical table
* Structured data for BI reporting
* Used `.to_sql()` for automated table refresh

Database: MySQL
Connector: SQLAlchemy

---

# 📊 Core Analytics

---

## 🔹 Sales & Revenue Analysis

* Monthly revenue trends
* Top-selling products
* Country-wise revenue
* Customer contribution analysis

---

## 🔹 RFM Customer Segmentation

RFM Metrics:

* Recency → Days since last purchase
* Frequency → Number of purchases
* Monetary → Total spending

Automated scoring (1–5 scale)

Generated segments such as:

* Champions
* Loyal Customers
* Promising
* At Risk
* Hibernating

---

## 🔹 Cohort Analysis

* Grouped customers by first purchase month
* Calculated retention rate over time
* Identified drop-off patterns

---

## 🔹 Market Basket Analysis

Used Apriori Algorithm:

* Support
* Confidence
* Lift

Identified product combinations for:

* Cross-selling
* Bundle strategy
* Promotion planning

Library: `mlxtend`

---

# ⚠️ Churn Intelligence System

---

## 🔸 Rule-Based Churn Risk

Churn classification using Recency logic:

* High Risk
* Medium Risk
* Low Risk

Business-driven explainable logic.

---

## 🔸 Revenue at Risk

Calculated:

* Total revenue from high-risk customers
* Revenue exposure percentage
* Top high-risk revenue contributors

---

## 🔸 Customer Priority Score

Combined:

* Monetary value
* Churn probability
* Risk weight

Generated ranked list of customers for retention strategy.

---

# 🤖 Machine Learning Churn Model

Built binary classification model to predict churn.

### Features Used:

* Recency
* Frequency
* Monetary
* RFM scores
* Customer priority score

### Outputs:

* `ML_Churn_Probability`
* `ML_Churn_Prediction`

### Model Evaluation:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

Applied probability calibration for realistic business interpretation.

---

# 🧠 Decision & Action Engine

Automated recommendation system:

| Condition                 | Recommended Action       |
| ------------------------- | ------------------------ |
| High churn + High value   | Immediate Retention Call |
| High churn + Medium value | Personalized Discount    |
| Medium churn              | Engagement Email         |
| Low churn                 | No Action                |

This transforms ML output into business strategy.

---

# 📈 Power BI Dashboard

Interactive Business Intelligence Dashboard includes:

* Revenue Overview
* Customer Segmentation Distribution
* Churn Risk Distribution
* Revenue at Risk KPI
* Customer Priority Ranking
* ML Churn Probability Visualization
* Country Performance Analysis

Power BI connected directly to MySQL for live refresh.

---

# 🔁 Automation System

The system supports automation:

### Automated Pipeline:

1. Data refreshed
2. Python script runs:

   * Cleaning
   * RFM
   * Churn logic
   * ML prediction
3. Table replaced in MySQL
4. Power BI auto-refreshes dashboard

Can be automated using:

* Windows Task Scheduler
* Cron Jobs
* Airflow (future scaling)

This enables near real-time decision intelligence.

---

# 🧰 Technologies Used

### Programming

* Python
* Jupyter Notebook

### Libraries

* pandas
* numpy
* scikit-learn
* mlxtend
* SQLAlchemy

### Database

* MySQL

### Visualization

* Power BI

---

# 📦 Final Outputs

* Structured SQL Data Warehouse
* Customer RFM Segmentation
* Churn Intelligence Table
* ML Probability Scores
* Revenue at Risk Analysis
* Automated Retention Recommendation
* Power BI Executive Dashboard

---

# 💼 Business Value

This system helps businesses:

* Reduce churn proactively
* Protect high-value customers
* Identify revenue leakage
* Improve retention ROI
* Prioritize marketing spend
* Make explainable ML decisions

---

# 🚀 Future Improvements

* Real-time streaming integration
* Advanced CLV modeling
* Model retraining automation
* Web-based dashboard deployment
* A/B testing retention strategies
* Deep learning churn modeling

---

# 👨‍💻 Author

**Deven Sorathiya**
PGD in Data Science & Analytics
Retail Analytics & ML Intelligence Project

---

# 📌 Conclusion

This project demonstrates a complete real-world analytics pipeline combining:

Data Engineering
Business Analytics
Machine Learning
Database Integration
Automation
Business Intelligence

Designed for scalable retail intelligence systems.

---
