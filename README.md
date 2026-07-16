# Enterprise Hotel Power BI Analytics

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow)
![DAX](https://img.shields.io/badge/DAX-Measures-blue)
![Data Modelling](https://img.shields.io/badge/Data%20Model-Star%20Schema-green)

## Overview

This project is an end-to-end **Power BI business intelligence solution** developed to analyse hotel financial performance, revenue drivers, cost structures, and operational profitability.

The dashboard transforms raw hotel financial data into interactive analytical insights that support management decision-making across revenue, costs, departments, booking channels, and market segments.

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

<img width="647" height="378" alt="02_Executive_Overview" src="https://github.com/user-attachments/assets/335a83a9-e1d4-484b-9b1d-c76d958b88e0" />



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

<img width="633" height="357" alt="03_Hotel_Performance_Analysis" src="https://github.com/user-attachments/assets/0c7b9071-1eb5-43dc-b9b1-0812cdce9168" />



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

<img width="654" height="377" alt="04_Revenue_Channel_Analysis" src="https://github.com/user-attachments/assets/9bdd3a3a-c712-41ed-91c2-62747ddb45bf" />



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

<img width="608" height="345" alt="05_Operational_Profitability" src="https://github.com/user-attachments/assets/7233cdc9-14a9-40f9-84bc-a54d48f33426" />



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

<img width="618" height="354" alt="06_Financial_Deep_Dive" src="https://github.com/user-attachments/assets/2b53a74f-2385-4dfd-a933-d37c8894dacb" />


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
DIVIDE(
    [Gross Profit],
    [Total Revenue],
    0
)
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
│   ├── Home_Page.png
│   ├── Executive_Overview.png
│   ├── Hotel_Performance.png
│   ├── Revenue_Channel_Analysis.png
│   ├── Operational_Analysis.png
│   └── Financial_Deep_Dive.png
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

**Renzo DG**

Data Analyst Portfolio Project

Tools:
Power BI | DAX | Power Query | SQL | R | Python
