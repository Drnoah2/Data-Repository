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





