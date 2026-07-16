# Enterprise Hotel Power BI Analytics

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow)
![DAX](https://img.shields.io/badge/DAX-Measures-blue)
![Data Modelling](https://img.shields.io/badge/Data%20Model-Star%20Schema-green)

## Overview

This project is an end-to-end **Power BI business intelligence solution** developed to analyse hotel financial performance, revenue drivers, cost structures, and operational profitability.

The dashboard transforms raw hotel financial data into interactive analytical insights that support management decision-making across revenue, costs, departments, booking channels, and market segments.

All data was AI generated and does not come from an actual hotel chain. It is all theoretical

The project demonstrates practical Data Analyst skills including:

- Data cleaning and transformation using Power Query
- Star schema data modelling
- DAX measure development
- Financial KPI analysis
- Interactive dashboard design
- Business insight generation

---

# Business Problem

Hotel management requires clear visibility into:

- Revenue performance across properties
- Cost drivers impacting profitability
- Department contribution to overall performance
- Effectiveness of booking channels
- Customer segment profitability

This dashboard was designed to answer:

> "What factors are driving hotel profitability, and where are opportunities to improve operational performance?"

---

# Tools & Technologies

| Tool | Purpose |
|---|---|
| Power BI | Dashboard development and data visualisation |
| DAX | KPI calculations and analytical measures |
| Power Query | Data cleaning and transformation |
| Data Modelling | Star schema architecture |
| Excel | Source data preparation |

---

# Dashboard Structure

## Home Page

Provides an introduction to the project and navigation across analytical sections.

<img width="622" height="347" alt="01_Home_Page" src="https://github.com/user-attachments/assets/b16a3f44-03aa-4e22-89e5-229675bd53ca" />



---

# Executive Overview

Provides a high-level summary of hotel performance.

Key metrics:

- Total Revenue
- Total Cost
- Gross Profit
- Gross Profit Margin %
- Revenue Growth %

Visuals include:

- Revenue trends
- Hotel performance comparison
- Profitability overview
- Revenue contribution analysis

<img width="647" height="364" alt="02_Executive_Overview" src="https://github.com/user-attachments/assets/dc3f7d80-be2d-4240-8284-2f5503dbb6d6" />



---

# Hotel Performance Analysis

Analyses performance differences between properties.

Key analysis:

- Revenue ranking by hotel
- Cost comparison
- Profit margin analysis
- Hotel profitability matrix

Business questions answered:

- Which hotels generate the highest revenue?
- Which properties deliver the strongest margins?
- Which hotels require further investigation?

<img width="633" height="357" alt="03_Hotel_Performance_Analysis" src="https://github.com/user-attachments/assets/47d1bf94-82bc-455d-8415-3538620a3699" />



---

# Revenue & Channel Analysis

Examines how revenue is generated through different customer acquisition channels.

Analysis includes:

- Booking channel revenue
- Market segment contribution
- Channel profitability
- Revenue trends by channel

Business questions answered:

- Are direct bookings more profitable?
- Which customer segments generate the most value?
- How does booking behaviour change over time?

<img width="654" height="368" alt="04_Revenue_Channel_Analysis" src="https://github.com/user-attachments/assets/0d9ed4df-e80f-4831-995b-e58bf8192b05" />


---

# Operational Profitability Analysis

Focuses on departmental performance and cost efficiency.

Analysis includes:

- Department revenue contribution
- Department profitability
- Cost allocation
- Operational efficiency

Departments analysed:

- Rooms
- Food & Beverage
- Spa
- Laundry
- Parking
- Conference & Events

<img width="608" height="337" alt="05_Operational_Profitability" src="https://github.com/user-attachments/assets/e7070dae-02ff-47e2-a91d-c7af47561b39" />



---

# Financial Deep Dive

Provides detailed financial analysis by showing how revenue converts into profit.

Includes:

- Revenue vs Cost trends
- Revenue-to-profit waterfall analysis
- Cost breakdown
- Financial summary tables

Key questions answered:

- Where are costs concentrated?
- Which departments impact profitability?
- Is revenue growth translating into profit growth?

<img width="618" height="345" alt="06_Financial_Deep_Dive" src="https://github.com/user-attachments/assets/f9931bc4-7881-472e-b03b-c4bffe5dd654" />



---

# Data Model

The project uses a **Star Schema data model** consisting of:

## Fact Table

### FactFinancials

Contains:

- Revenue
- Cost
- Date
- Hotel
- Department
- Booking Channel
- Market Segment


## Dimension Tables

|Table|Purpose|
|-|-|
|DimDate|Time intelligence and trend analysis|
|DimHotel|Hotel-level reporting|
|DimDepartment|Department analysis|
|DimBookingChannel|Revenue source analysis|
|DimMarketSegment|Customer analysis|

Model structure:

```
                 DimDate
                    |
                    |
DimHotel ---- FactFinancials ---- DimDepartment
                    |
                    |
          DimBookingChannel
                    |
                    |
          DimMarketSegment
```

---

# Key DAX Measures

The dashboard uses calculated measures rather than static calculations.

Examples:

## Total Revenue

```DAX
Total Revenue =
SUM(FactFinancials[Revenue])
```

## Gross Profit

```DAX
Gross Profit =
[Total Revenue] - [Total Cost]
```

## Gross Profit Margin

```DAX
Gross Profit Margin % =
DIVIDE([Gross Profit], [Total Revenue], 0)
```

---

# Key Business Insights

Example insights generated from the analysis:

### Revenue Performance

- Identified the highest revenue-generating hotels and departments.
- Analysed monthly revenue patterns and seasonal trends.

### Profitability

- Compared revenue growth against cost growth to evaluate profitability.
- Identified areas where high revenue did not translate into strong margins.

### Operational Efficiency

- Analysed department-level cost contribution.
- Highlighted opportunities for improving cost efficiency.

### Customer & Channel Strategy

- Evaluated booking channel profitability.
- Compared customer segment contribution.

---

# Project Files

```
Enterprise-Hotel-PowerBI-Analytics

│
├── README.md
│
├── PowerBI
│   └── Enterprise_Hotel_Analytics.pbix
│
├── Documentation
│   ├── Business_Requirements_Document.pdf
│   ├── KPI_DAX_Measure_Library.pdf
│   └── Data_Model_Documentation.pdf
│
├── Screenshots
│   ├── 01_Home_Page.png
│   ├── 02_Executive_Overview.png
│   ├── 03_Hotel_Performance.png
│   ├── 04_Revenue_Channel_Analysis.png
│   ├── 05_Operational_Analysis.png
│   └── 06_Financial_Deep_Dive.png
│   └── 07_Data_Model_Star_Schema
```

---

# Skills Demonstrated

✔ Power BI Dashboard Development  
✔ DAX Measure Creation  
✔ Data Modelling  
✔ Power Query Transformation  
✔ Financial Analysis  
✔ Business Intelligence Reporting  
✔ Data Storytelling  

---

# Author

**Renzo Del Grosso**

Data Analyst Portfolio Project

Tools:
Power BI | DAX | Power Query
