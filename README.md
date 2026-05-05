# 📊 Credit Card Financial Dashboard (Power BI)

An interactive **Credit Card Financial Dashboard** built using **Power BI**, **SQL**, and **data modeling** to analyze customer behavior, revenue trends, and credit card performance metrics.  
This project provides **real-time insights** for stakeholders to support business decisions and monitor financial performance.

---

## 🚀 Project Overview

This dashboard helps analyze:

- Revenue trends (weekly, monthly, quarterly)
- Customer behavior & demographics
- Transaction patterns
- Interest earned, annual fees, and revolving balance
- Credit card usage (chip, swipe, online)
- Customer segmentation by age, salary, job role, education, etc.
- State-wise performance contribution
- KPIs such as total income, total interest, customer satisfaction score (CSS), delinquency rate, activation rate

---

## 🎯 Objective

To build a **comprehensive, data-driven dashboard** enabling financial teams and decision-makers to monitor:

- Key performance indicators (KPIs)
- Customer insights
- Transaction behavior
- Revenue contribution by segments
- Week-over-week and year-to-date growth patterns

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| **Power BI** | Dashboard design, DAX calculations, data visualization |
| **SQL (PostgreSQL / MySQL)** | Data cleaning, transformation, and extraction |
| **Excel/CSV** | Source data |
| **DAX** | Custom KPIs, measures, hierarchies |
| **Data Modeling** | Relationship creation and ETL pipeline |

---

## 📂 Dataset Details

The project uses two datasets:

### **1️⃣ Transaction Dataset (`cc_detail`)**
Contains weekly transaction data:
- Client number
- Card category
- Annual fees
- Customer acquisition cost
- Week number & week start date
- Total transaction amount
- Transaction count
- Interest earned
- Delinquency indicator  
…and more.

### **2️⃣ Customer Dataset (`cust_detail`)**
Includes customer-level information:
- Age  
- Gender  
- Marital status  
- Income  
- Job role  
- Education  
- Customer satisfaction score  
- Loan/house/car ownership  
…and more.

---

## 🧩 SQL Scripts (Data Import & Cleaning)

SQL file used:  
**`SQL Query - Financial Dashboard Data.sql`**

Key steps include:

- Creating database `ccdb`
- Creating tables `cc_detail` and `cust_detail`
- Importing CSVs using `COPY` command
- Handling date formatting and cleaning issues
- Creating calculated fields for analysis

```sql
CREATE DATABASE ccdb;

CREATE TABLE cc_detail (...);
CREATE TABLE cust_detail (...);

COPY cc_detail FROM 'credit_card.csv' DELIMITER ',' CSV HEADER;
COPY cust_detail FROM 'customer.csv' DELIMITER ',' CSV HEADER;
I worked on was a Credit Card Financial Dashboard, where the objective was to analyze customer transaction and financial data to track key business KPIs.

The dataset contained over 100,000 customer and transaction records, including spending patterns, payment behavior, and customer segments.

The goal of this project was to build an interactive dashboard that could help monitor financial performance, customer behavior, and credit-related risk indicators.

For this project, I used SQL for data extraction and transformation, and Power BI for dashboard development and visualization.

I created dashboards to track key KPIs such as total spend, transaction trends, default rate, customer segmentation, and spending behavior across different customer groups.

I also worked on data modeling, KPI calculations, and interactive filters so users could analyze trends dynamically.

As an outcome, the dashboard made it easier to monitor customer financial behavior, identify risk trends, and support data-driven decisions related to customer targeting and credit performance
