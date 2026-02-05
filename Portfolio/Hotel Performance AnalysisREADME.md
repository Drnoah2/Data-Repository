# Hotel Performance Analysis (2018-2020)
---
# Table of Content
---
- [Introduction](#introduction)
- [Problem Statement](#problem-statement)
- [Data Sourcing](#data-sourcing)
- [Data Transformation & Cleaning](#data-transformation-&-cleaning)
- [Data Modeling](#data-modeling)
- [Data Analysis](#data-analysis)
- [Data Visualization](#data-visualization)
- [Conclusion](#conclusion)
- [Recommendation](#recommendation)


---
## Introduction
---
This project presents a Hotel Performance Analysis Dashboard built using Power BI, designed to provide an overview of hotel booking patterns, guest demographics and operational efficencies, in order to maximize revenue.


---
## Problem Statement
---
Hotel management faces challenges in:
- Tracking overall revenue performance over time
-	Identifying top-performing markets and countries
-	Understanding guest demographics and booking patterns
-	Monitoring pricing effectiveness (ADR) and booking demand
Without a centralized analytical view, decision-making becomes reactive rather than proactive.
This project aims to solve this by transforming raw hotel booking data into an interactive and insightful Power BI dashboard.


---
## Data Sourcing
---
The data was sourced as structured tables from google spreadsheet in an excel file format and imported into Power BI Desktop for analysis.
<img width="1357" height="606" alt="image" src="https://github.com/user-attachments/assets/2bcbdfb6-6bbf-4e03-8a33-0d3fbe314717" />
While the location and country was done through data scraping from the link below;
https://statisticstimes.com/geography/countries-by-continents.php


---
## Data Transformation & Cleaning
---
Data preparation was carried out using Power Query, including:
-	Removing duplicates, errors and null values
-	Standardizing column names and formats
-	Converting date fields into a dedicated Date Dimension
-	Creating calculated measure for revenue-related metrics
-	Ensuring consistency in the fact and dimension tables
-	Ensuring the right data type was used for all the columns
These steps ensured data accuracy, reliability, and readiness for modeling.
Attached here are the applied steps carried out in the power query during the cleaning and transformation
<img width="1758" height="863" alt="image" src="https://github.com/user-attachments/assets/7772a602-9f3e-45d8-82c7-5890e3333f35" />


---
## Data Modeling
---
A star schema was implemented to improve performance and usability:
•	Fact Table: Hotel Fact (bookings, revenue, ADR, waiting days)
•	Dimension Tables: Date Dimension, Hotel Dimension, Location Dimension, Market Segment, Meal Cost
The relationship between the fact and the dimension table was based on one to many cardinality.
Attached below is the star schema of the modeling structure
<img width="857" height="482" alt="image" src="https://github.com/user-attachments/assets/9a5f2bc7-3a9d-4941-8b00-71d1da8ee15f" />


---
## Data Analysis
---
### Key Insights
-	Total Revenue: ₦49.67M, indicating strong overall performance.
-	Seasonality: Revenue peaks around July–August, suggesting high seasonal demand.
-	Top Revenue Country: Portugal leads significantly, followed by Great Britain and France.
-	Customer Contribution:
-	Transient customers contribute the largest share of revenue.
-	Group and contract bookings play a smaller but stable role.
-	Average Daily Rate (ADR): 99.42, indicating competitive pricing.
-	Waiting List Duration: Low average (2.31 days), suggesting efficient booking management.

---

## Monthly Revenue Trend

**Chart Type:** Line Chart
**Metric:** Total Monthly Revenue

### Key Insights

* Revenue begins at a moderate level in **January (~₦3.4M)** and dips in **February**, indicating post-holiday slowdown.
* A steady upward trend is observed from **March to June**, reflecting recovering demand.
* **Peak revenue occurs in August (~₦7.5M)**, showing strong seasonal performance.
* A sharp decline begins in **September**, with **December recording the lowest revenue (~₦2.26M)**.
* Revenue volatility suggests strong **seasonal dependence**.

### Recommendations

* Implement **dynamic pricing** to maximize revenue during peak months (July–August).
* Introduce **off-season discounts and bundled offers** between September and February.
* Align staffing, inventory, and marketing spend with seasonal demand cycles.
* Use historical trends to improve **forecasting and capacity planning**.

---

## Customers’ Days in Waiting List

**Chart Type:** Pie Chart
**Metric:** Average Days in Waiting List by Customer Type

### Key Insights

* **Transient customers** account for the highest waiting time (**~6.04 days**).
* **Transient-Party customers** experience moderate waiting time (**~1.26 days**).
* **Group customers** have minimal waiting periods (**~0.28 days**).
* **Contract customers** show negligible waiting time, suggesting priority access.

### Recommendations

* Improve room availability forecasting for **transient demand**, especially during peak seasons.
* Introduce **real-time waitlist updates** to improve customer experience.
* Reassess allocation rules to reduce waiting time without impacting high-value bookings.
* Consider converting long-waiting transient guests into future bookings through incentives.

---

## Top Five Countries With Most Revenue

**Chart Type:** Horizontal Bar Chart
**Metric:** Revenue by Country

### Key Insights

* **Portugal** is the top contributor, generating **₦18.0M**, far exceeding other countries.
* **Great Britain** ranks second with **₦5.9M**, followed by France, Spain, and Germany.
* Revenue contribution declines sharply after the top country.
* Heavy reliance on one market increases **geographic concentration risk**.

### Recommendations

* Strengthen customer retention strategies in **Portugal** to sustain dominance.
* Expand targeted marketing campaigns in **Great Britain and France**.
* Explore growth opportunities in underperforming regions through localized promotions.
* Diversify revenue sources to reduce dependency on a single country.

---

## Revenue by Customers

**Chart Type:** Donut Chart
**Metric:** Revenue Contribution by Customer Type

### 🔍 Key Insights

* **Transient customers** generate the majority of revenue (**~₦38.43M**).
* **Transient-Party customers** contribute a notable share (**~₦8.3M**).
* **Group customers** generate relatively low revenue (**~₦2.76M**).
* **Contract customers** contribute the least overall.

### Recommendations

* Reduce over-reliance on transient bookings by growing **group and contract segments**.
* Design customized pricing and incentives for long-stay and corporate customers.
* Increase group booking promotions during low-demand periods.
* Balance the customer mix to improve revenue stability.

---

## Overall Business Implications

* Hotel performance is **highly seasonal**, with revenue peaks concentrated in mid-year.
* **Transient customers** dominate both revenue and operational pressure.
* Revenue is **geographically concentrated**, increasing exposure to market shifts.
* Waiting list data reveals opportunities to improve operational efficiency.

---

## Conclusion

The chart-level analysis highlights strong revenue potential driven by seasonality and transient demand, alongside risks related to customer and geographic concentration. By diversifying customer segments, optimizing pricing strategies, and improving waitlist management, the hotel can achieve more stable and sustainable revenue growth.


---
## Data Visualization
---
The Power BI dashboard includes:
- KPI Cards for quick performance overview
-	Monthly Revenue Trend Line Chart to analyze seasonality
-	Bar Charts showing revenue by top five countries
-	Column Chart illuistrating average waiting list days by customer type
-	Donut Chart illustrating revenue distribution by customer type
-	Interactive filters for dynamic analysis
---
<img width="1342" height="752" alt="image" src="https://github.com/user-attachments/assets/3951c5bd-d981-40a0-8616-dac2cc7c2fac" />


---
## Conclusion
---
This project demonstrates how raw hotel booking data can be transformed into meaningful business intelligence using Power BI to generate more insight on the guest demographics, operational efficeincies and booking patterns in the industry by integrating data cleaning, modeling, analysis, and visualization, the dashboard provides actionable insights that support revenue optimization and strategic planning.


---
## Recommendation
---







