# Hospitality Revenue & Occupancy Analytics

End-to-end analysis of 134K+ hotel bookings across 4 Indian cities (May–Jul 2022), combining Python EDA with a Power BI executive dashboard to uncover pricing, cancellation, and service-quality inefficiencies.

## Overview
<p align="center">
  <img src="images/Dashboard.png" width="800"/>
</p>

<p align="center">
  <img src="images/ADR_vs_occ_pct.jpeg" width="800"/>
</p>

* Domain - Hospitality / Hotel Revenue Management
* Tools - Python (Pandas, Matplotlib, Seaborn), Power BI, DAX
* Dataset - 5 tables · 134,576 bookings · 25 properties · 4 cities
* Deliverables - Jupyter Notebook (EDA) + Power BI Dashboard (.pbix)

---

## Objective
Hotels track revenue and occupancy separately, but rarely look at how the two interact. This project asks one question:
* Is revenue being lost because of low demand, or because of how rooms are priced and managed?
The objective is to help hotel management teams optimize pricing, improve occupancy, and maximize revenue using data-driven insights.

---

## Business Problem

The hospitality industry faces challenges in maximizing revenue while balancing occupancy, pricing, and booking efficiency.

Management required a centralized solution to:
* Monitor revenue performance across properties and cities.
* Track KPIs such as RevPAR, ADR, Occupancy %, and Realization %.
* Identify revenue leakage caused by cancellations and no-shows.
* Understand customer behavior and booking patterns.
* Support pricing and demand-management decisions.

---

## Part 1 — Python EDA
Notebook: [`Hospitality_Analysis.ipynb`](https://github.com/adityadhiman96/PowerBI-Hospitality-Revenue-Performance-Dashboard/blob/main/notebook/Hospitality_Analysis.ipynb)
* Data Cleaning
  - Removed records with invalid `no_guests` (≤0) — <1% of data
  - Applied the 3-sigma rule to detect and remove outliers in `revenue_generated`
  - Validated `revenue_realized` outliers against room category (RT4 / Presidential) before deciding not to remove them — avoided over-cleaning legitimate       luxury pricing
  - Filled missing `capacity` values using median
  - Removed rows where `successful_bookings > capacity` (logically invalid)
  - Retained ~80K null values in `ratings_given` rather than imputing — avoided distorting guest sentiment data

* KPIs Engineered
  - ADR (Average Daily Rate)	Total Revenue ÷ Total Bookings
  - RevPAR (Revenue per Available Room)	Total Revenue ÷ Total Capacity
  - Occupancy %	Successful Bookings ÷ Capacity × 100
  - Realization %	Revenue Realized ÷ Revenue Generated × 100
  - Cancellation Rate	Cancelled Bookings ÷ Total Bookings × 100

* Independent Analysis (Ad-Hoc)
  - Occupancy by room class, city, and weekday vs. weekend
  - Month-on-month revenue trends
  - ADR vs. Occupancy % — dual-axis monthly trend
  - Revenue per booking by platform
  - Cancellation rate by city
  - Rating distribution by room class (Seaborn boxplot)



---

## Key Insights

* Revenue declined by ~22% despite stable occupancy, indicating pricing inefficiencies
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
