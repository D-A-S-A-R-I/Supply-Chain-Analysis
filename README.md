# Supply-Chain-Analysis
Power BI dashboard analyzing supply chain operations, logistics performance, and inventory insights

# 📦 Supply Chain Analysis Dashboard
## 📌 Project Overview

This project focuses on analyzing supply chain data to understand order trends, revenue performance, and overall operational efficiency. The dashboard provides interactive insights into sales, orders, and time-based performance to support business decision-making.

---

## 🎯 Objective

The main objectives of this project are:

* Analyze order and revenue performance
* Track business growth over time
* Identify trends and patterns in supply chain data
* Provide insights for improving operational efficiency

---

## 📂 Dataset Description

The dataset includes:

* Order details
* Product information
* Revenue data
* Date and time information
* Location-based attributes

---

## 🧹 Data Cleaning & Preparation

The data was prepared using the following steps:

* Removed duplicate records
* Handled missing/null values
* Standardized date and number formats
* Cleaned inconsistent values
* Structured the dataset for analysis

---

## 📊 Data Modeling

* Created relationships between tables
* Structured the data model for reporting
* Ensured proper filtering across visuals

---

## 📐 DAX Calculations Used

* **Total Orders**

```DAX id="a1"
Total Orders = COUNT(Orders[Order ID])
```

* **Total Revenue**

```DAX id="a2"
Total Revenue = SUM(Orders[Revenue])
```

* **Total Cost**

```DAX id="a3"
Total Cost = SUM(Orders[Cost])
```

* **Profit**

```DAX id="a4"
Profit = [Total Revenue] - [Total Cost]
```

* **Average Revenue**

```DAX id="a5"
Average Revenue = AVERAGE(Orders[Revenue])
```

* **Month-over-Month Growth**

```DAX id="a6"
MoM Growth = 
DIVIDE(
    [Total Revenue] - CALCULATE([Total Revenue], PREVIOUSMONTH(Orders[Order Date])),
    CALCULATE([Total Revenue], PREVIOUSMONTH(Orders[Order Date])),
    0
)
```

* **Year-over-Year Growth**

```DAX id="a7"
YoY Growth = 
DIVIDE(
    [Total Revenue] - CALCULATE([Total Revenue], SAMEPERIODLASTYEAR(Orders[Order Date])),
    CALCULATE([Total Revenue], SAMEPERIODLASTYEAR(Orders[Order Date])),
    0
)
```

---

## 📈 Dashboard Features

* **KPI Cards**

  * Total Orders
  * Total Revenue
  * Profit

* **Time-Based Analysis**

  * Monthly trends
  * Year-over-Year comparison

* **Category Analysis**

  * Performance by product/category

* **Regional Insights**

  * Sales distribution by location

* **Interactive Filters**

  * Date
  * Category
  * Region

* **Drill-through Analysis**

  * Detailed breakdown of performance

---

## 🔍 Key Insights

* Identified revenue trends over time
* Observed business growth patterns using YoY and MoM
* Highlighted top-performing categories and regions
* Provided insights into overall business performance

---

## 💼 Business Impact

This dashboard helps businesses to:

* Monitor performance effectively
* Understand growth trends
* Identify high-performing areas
* Support strategic decision-making

---

## 📁 Files Included

* 📄 Supply Chain Analysis Report (PDF)
* 📊 Presentation (PPT)
* 📈 Dashboard File
* 📂 Dataset
* 🖼️ Dashboard Screenshots

---

## 👨‍💻 Roles & Responsibilities

* Understood business requirements
* Cleaned and transformed raw data
* Built data model and relationships
* Created DAX measures for KPIs
* Designed interactive dashboard
* Generated business insights

---

## 🚀 Conclusion

This project demonstrates the ability to analyze business data, track performance trends, and build interactive dashboards to support decision-making.



