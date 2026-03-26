# 🏨 Hospitality Revenue Performance Dashboard (Power BI)

## 📌 Overview

This project analyzes hotel performance across multiple cities to identify revenue decline, pricing inefficiencies, and booking behavior patterns.

The dashboard focuses on answering:

* What is happening to revenue?
* Why is performance declining?
* What actions can improve profitability?

---

## 🎯 Business Problem

The hospitality business is experiencing a **decline in revenue despite stable occupancy levels**.
The objective is to identify root causes and recommend data-driven strategies to improve performance.

---

## 📊 Key Metrics Used

* **Revenue**
* **RevPAR (Revenue per Available Room)**
* **ADR (Average Daily Rate)**
* **DBRN (Daily Bookable Room Nights)**
* **DSRN (Daily Sellable Room Nights)**
* **DURN (Daily Utilized Room Nights)**
* **Occupancy %**
* **Realisation %**

---

## 🔍 Key Insights

* Revenue declined by **~22% WoW**, while occupancy remained relatively stable
* Indicates **pricing inefficiency (ADR misalignment)**
* High **cancellations and no-shows** are reducing realised revenue
* **Hyderabad** underperforms in RevPAR compared to other cities
* Weekends perform better > demand is unevenly distributed

---

## 🚀 Recommendations

* Implement **dynamic pricing strategy (demand-based ADR)**
* Introduce **prepaid booking incentives** to reduce cancellations
* Improve **weekday occupancy** through targeted offers
* Focus on **underperforming cities & properties**

---

## 🌐 Live Dashboard

👉 [Click here to view the interactive dashboard](https://app.powerbi.com/view?r=eyJrIjoiZDMxYTQyODgtZGRiZC00ZjFlLWEzYzAtMzM5ZDEzZTEwZmNkIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9))

---

## 🛠 Tools & Skills

* Power BI
* DAX (Calculated Measures, KPIs)
* Data Visualization & Dashboard Design
* Business Analysis (Hospitality Domain)

---

## 📷 Preview

* [Dashboard](images/Dashboard.png)
* [Data Model](images/Data_Model.png)

---

## 📂 Dataset & Data Modeling

* Analyzed 10,000+ records of hotel booking data
* Designed a Star Schema data model for efficient analysis

---

## 🔗 Relationships:

* One-to-Many relationships from dimension tables to fact table
* Enabled fast aggregations and scalable analysis

---

## ⚙️ Data Modeling Approach
* Cleaned and transformed raw data using Power Query
* Built a star schema to improve performance and simplify DAX
* Created measures instead of calculated columns for flexibility
* Used context-aware DAX for KPIs like RevPAR, ADR, and Occupancy

---

## 💡 What I Learned

* Translating business problems into analytical dashboards
* Identifying revenue drivers using KPIs like RevPAR & ADR
* Designing dashboards for **decision-making, not just visualization**

---
