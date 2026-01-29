# 🛒 Retail Customer Analytics & Churn Intelligence

## 📌 Project Overview

This project focuses on analyzing retail transaction data to understand **customer behavior, sales performance, churn risk, and revenue impact**. The objective is to help retail businesses **identify high-risk customers, prioritize retention efforts, and make data-driven decisions** using analytics and machine learning.

---

## 🎯 Business Problem

Retail businesses commonly struggle to:

* Identify **high-value customers**
* Detect **early signs of customer churn**
* Understand which customer segments **generate or risk losing revenue**
* Decide **where to focus retention efforts** effectively

This project addresses these challenges using **structured data analysis, churn intelligence, and predictive modeling**.

---

## 🗂️ Data Source

* Retail transaction dataset containing:

  * Invoices
  * Products
  * Customers
  * Transaction dates
  * Quantities
  * Prices
* Data processed using **Python** and stored in a **MySQL database** for scalable analysis

---

## ⚙️ Key Steps Performed

### 1️⃣ Data Cleaning & Preparation

* Removed invalid and negative quantity records
* Handled missing customer IDs
* Created **total transaction amount** feature
* Converted date fields into usable **time-based features**
* Ensured clean, consistent, and analysis-ready data

### 2️⃣ SQL Integration

* Stored cleaned and transformed data in **MySQL**
* Created analytical tables for **customer-level insights**
* Used SQL queries for structured validation and analysis

---

## 📊 Core Analytics Performed

### 🔹 Sales & Revenue Analysis

* Monthly sales trend analysis
* Top-selling products by quantity and revenue
* Country-wise revenue aggregation

### 🔹 Customer Analytics (RFM)

* RFM Analysis:

  * **Recency** – How recently a customer purchased
  * **Frequency** – How often they purchase
  * **Monetary** – How much they spend
* Automated RFM scoring (scale 1–5)
* Customer segmentation based on RFM scores

### 🔹 Cohort Analysis

* Grouped customers by **first purchase month**
* Analyzed customer retention behavior over time

### 🔹 Market Basket Analysis

* Applied **Apriori Algorithm** for association rule mining
* Identified frequently purchased product combinations
* Generated rules using:

  * Support
  * Confidence
  * Lift

---

## ⚠️ Risk & Retention Intelligence

### 🔸 Churn Risk Scoring

* Rule-based churn logic using recency and purchase behavior
* Classified customers into:

  * High Risk
  * Medium Risk
  * Low Risk

### 🔸 Revenue at Risk

* Calculated potential revenue loss from high-risk customers

### 🔸 Customer Priority Score

* Combined churn risk with monetary value
* Ranked customers by overall **business importance**

---

## 🤖 Machine Learning (Churn Model)

* Built a **binary churn prediction model**
* Trained and evaluated using classification metrics
* Generated churn probabilities for each customer
* Applied **probability calibration** for realistic and reliable risk scoring

---

## 🧠 Advanced Decision Logic

### 🔹 Rule-Based vs ML Churn Comparison

* Compared traditional business rules with ML-based predictions
* Identified agreement and disagreement cases

### 🔹 Decision Threshold Optimization

* Tuned churn probability thresholds for improved business decisions

### 🔹 Action Recommendation Engine

Based on churn probability and customer priority, recommended actions such as:

* Immediate Retention Call
* Personalized Discount
* Engagement Email
* No Action Needed

---

## 🧰 Technologies Used

* **Python**: pandas, numpy, scikit-learn, mlxtend
* **SQL / MySQL**
* **Machine Learning**: classification models, probability calibration
* **Jupyter Notebook**

---

## 📦 Final Outputs

* Cleaned and structured **SQL database**
* Customer segmentation and churn intelligence tables
* Revenue-at-risk and customer priority scoring
* Actionable insights to support **retention strategy**

---

## 💡 Project Value

This project demonstrates how **data analytics and machine learning** can be combined to:

* Reduce customer churn
* Protect and optimize revenue
* Support business decision-making with **clear and explainable insights**

---

## 🚀 Future Improvements

* Real-time data integration
* Continuous model retraining with new data
* A/B testing of retention strategies
* Advanced **Customer Lifetime Value (CLV)** modeling

---

📌 *This project is designed to be practical, business-focused, and scalable for real-world retail analytics use cases.*
