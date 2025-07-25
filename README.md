# 📊 End-to-End Project Documentation & Analytical Summary

## Table of Contents
- [Introduction](#introduction)  
- [Data Preparation & Structure](#data-preparation--structure)  
- [Analytical Approach](#analytical-approach)  
- [Dashboard Features & Insights](#dashboard-features--insights)  
  - [Home Overview](#home-overview)  
  - [Loan Analysis](#loan-analysis)  
  - [Deposit Analysis](#deposit-analysis)  
  - [Client Risk & Exposure Summary](#client-risk--exposure-summary)  
- [Functions & Techniques Used](#functions--techniques-used)  
- [Visuals from the Dashboard](#visuals-from-the-dashboard)  
- [Conclusion](#conclusion)  

---

## 📌 Introduction
The Banking Risk Analysis Dashboard is designed for comprehensive bank data evaluation and risk monitoring. It integrates data from a MySQL database originally derived from Excel files, utilizing robust Python-based ETL and analytics processes. The dashboard supports multidimensional analysis of lending and deposit activity, risk segmentation, and customer profiling through a dynamic, user-friendly interface.

## 🧱 Data Preparation & Structure
Customer banking records were imported from CSV or Excel files into a MySQL database (`banking_cases.customer`), supporting relational queries and efficient ETL.

SQLAlchemy and Pandas in a Jupyter Notebook provided secure data access, preprocessing, and transformation.

The dataset contains:

- **Client Demographics:** ID, Name, Age, Gender, Nationality, Occupation  
- **Account Info:** Join Date, Branch ID, Banking Contact  
- **Financial Products:** Estimated Income, Superannuation, Credit Card Balances, Loans, Deposits, Checking/Saving Accounts, Business Lending, Property Holdings  
- **Risk Features:** Risk Weighting, Default Rate, High Risk Status, Risk Category/Score, Loyalty Classification  

Data preparation involved handling missing values and standardizing datatypes (dates, numerics). Derived features such as risk category and loyalty classifications were created, along with validation for uniqueness and consistency across key identifiers.

## 🧠 Analytical Approach
Targeted SQL queries were executed to extract both granular customer records and summarized aggregates.

Data cleaning using Pandas addressed missing values, performed data type casting, and corrected inconsistencies.

Functions were developed for portfolio KPIs, including total loan and deposit amounts, default and high-risk ratios, average risk scores, and segment distributions.

Grouping and aggregation were performed by client demographics, financial product type, banking relationship, income, and risk brackets.

Interactive and filterable visuals were designed in Power BI using a variety of chart types and customizable pages.

---

## 📊 Dashboard Features & Insights

### 🏠 Home Overview
![Home Overview](images/Home%20Overview.png)

### 💳 Loan Analysis
![Loan Analysis](images/Loan%20Analysis.png)

### 💰 Deposit Analysis
![Deposit Analysis](images/Deposit%20Analysis.png)

### ⚠️ Client Risk & Exposure Summary
![Risk Summary](images/Risk%20Summary.png)

---

## 🛠️ Functions & Techniques Used

### Python & Jupyter Notebook
- Libraries used: `sqlalchemy`, `pandas`, `matplotlib`, `seaborn`  
- Secure database connections with SQLAlchemy  
- Data queried using `pd.read_sql()`  
- Aggregations, groupings, and cleaning using `pandas`  
- Exported summaries to Power BI

### Power BI
- Dashboard Pages: Home, Loan Analysis, Deposit Analysis, Risk Summary  
- DAX Measures: Totals, averages, flags, responsive metrics  
- Visual Types: KPI cards, bar charts, pie charts, line graphs, scatter plots  
- Filters: Year, Gender, Relationship Type, Advisor

---

## 🖼️ Visuals from the Dashboard

### 📌 Jupyter Notebook Visuals

#### 📈 Risk Score Distribution
![Risk Score Distribution](images/Risk%20Score%20Distribution.png)

#### 📉 Default Rate by Age Group
![Default Rate by Age Group](images/Default%20Rate%20by%20Age%20Group.png)

#### 📊 Loan vs Deposit Ratio
![Loan vs Deposit Ratio](images/Loan%20vs%20Deposit%20Ratio.png)

#### 🧮 Risk Category Segmentation
![Risk Category Segmentation](images/Risk%20Category%20Segmentation.png)

---

## ✅ Conclusion
The Banking Risk Analysis Dashboard integrates MySQL, Python, and Power BI to provide actionable insights on client portfolios, risk exposure, and financial product performance. Its modular design enables targeted analysis and rapid identification of risk trends, supporting effective, data-driven decisions for banking operations and risk management.

---

### 🧰 Tools Used:
- **MySQL**  
- **Jupyter Notebook** (`Pandas`, `SQLAlchemy`, `Matplotlib`, `Seaborn`)  
- **Power BI** (`DAX`, custom visuals, navigation buttons, slicers`)


## 📁 Power BI Dashboard File

You can download and open the full interactive dashboard using Power BI Desktop:

📊 **[Banking Risk Analysis Dashboard.pbix](./Banking%20Risk%20Analysis%20Dashboard.pbix)**  
➡️ *Click “Download” or “View raw” on the next page to save the file.*  
📦 _(File size: ~3MB, Power BI required to view)_
