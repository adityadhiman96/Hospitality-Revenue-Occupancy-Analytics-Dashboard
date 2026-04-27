# Hospitality Revenue Performance Dashboard (Power BI)

## Overview
<p align="center">
  <img src="images/Dashboard.png" width="800"/>
</p>

This project presents an end-to-end Power BI dashboard built to analyze hospitality revenue performance across multiple cities, properties, and booking channels.

The objective is to help hotel management teams optimize pricing, improve occupancy, and maximize revenue using data-driven insights.

---

## Business Problem

The hospitality business is experiencing a **decline in revenue despite stable occupancy levels**.
The objective is to identify root causes and recommend data-driven strategies to improve performance.

---

## Key Metrics Used

* Revenue: 1.70Bn
* RevPAR: 7.41K
* Occupancy Rate: 57.8%
* ADR (Average Daily Rate): 12.69K
* Realization Rate: 70.1%

---

## Key Insights

* Revenue declined by ~22% despite stable occupancy → indicates pricing inefficiencies
* Weekends show same ADR and RevPAR as weekdays, indicating static pricing strategy
* High cancellations & no-shows (~40K+) are significantly impacting realized revenue
* Mumbai leads in revenue generation, while some cities underperform in RevPAR
* Hyderabad shows lower RevPAR, indicating an underperforming market
* Luxury category contributes higher revenue compared to business hotels

---

## Dashboard Features
* Dynamic time filtering (Week-wise analysis)
* City & Property-level drill-down
* Room class segmentation
* Trend analysis of key metrics
* Performance matrix (ADR vs Occupancy)
* Day-type comparison (Weekday vs Weekend)

---

## Data Model
* Designed using Star Schema for performance optimization
* Tables:
  Fact Table - Bookings, Aggregated_Bookings
  Dimension Tables - Date, Hotels, Room

---

## Tools & Skills
* Power BI
* DAX (Data Analysis Expressions)
* Data Modeling
* Business Intelligence

---

## Recommendations

* Implement dynamic pricing strategies based on demand
* Increase prices during high-demand weekends
* Reduce cancellations through advance booking incentives
* Improve underperforming markets (e.g., Hyderabad)
* Focus on optimizing RevPAR instead of just occupancy

---

## Live Dashboard

[Click here to view the interactive dashboard](https://app.powerbi.com/view?r=eyJrIjoiZDMxYTQyODgtZGRiZC00ZjFlLWEzYzAtMzM5ZDEzZTEwZmNkIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)

---

## Preview

* [Dashboard](images/Dashboard.png)
* [Data Model](images/Data_Model.png)

---

## Dataset & Data Modeling

* Analyzed 10,000+ records of hotel booking data
* Designed a Star Schema data model for efficient analysis

---

## Relationships:

* One-to-Many relationships from dimension tables to fact table
* Enabled fast aggregations and scalable analysis

---

## Data Modeling Approach
* Cleaned and transformed raw data using Power Query
* Built a star schema to improve performance and simplify DAX
* Created measures instead of calculated columns for flexibility
* Used context-aware DAX for KPIs like RevPAR, ADR, and Occupancy

---

## What I Learned

* Translating business problems into analytical dashboards
* Identifying revenue drivers using KPIs like RevPAR & ADR
* Designing dashboards for **decision-making, not just visualization**

---

## Author
Aditya Dhiman
