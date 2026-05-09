# ☕ Coffee Shop Sales Analysis Dashboard

## 📌 Project Overview

This project focuses on analyzing retail coffee shop sales data using Microsoft Excel to generate actionable business insights and improve overall store performance.

An interactive dashboard was created to track sales trends, customer behavior, product performance, and store-level analysis.

---

# 🎯 Project Objective

The main objective of this project is to analyze coffee shop retail sales data and provide meaningful insights that help improve:

* Sales performance
* Customer purchasing behavior
* Product strategy
* Store operations
* Revenue growth

---

# 📊 Business Questions Solved

1. How do sales vary by day of the week and hour of the day?
2. Are there any peak times for sales activity?
3. What is the monthly sales revenue trend?
4. How do sales vary across different store locations?
5. What is the average bill value and average order per customer?
6. Which products are best-selling in terms of quantity and revenue?
7. How do sales vary by product category and size?

---

# 🛠 Tools & Techniques Used

* Microsoft Excel
* Pivot Tables
* Pivot Charts
* Slicers
* KPI Cards
* Data Cleaning
* Conditional Formatting
* Dashboard Design

---

# 📈 Key KPIs

* Total Sales
* Total Footfall
* Average Bill Per Person
* Average Orders Per Person
* Top Product
* Sales by Store Location
* Sales by Product Category
* Hourly Sales Trends

---

# 🔍 Key Insights

* Morning hours generated the highest sales activity.
* Coffee category contributed the maximum share of revenue.
* Hell’s Kitchen store recorded the highest sales performance.
* Top-selling products significantly influenced overall revenue.
* Weekday sales trends showed consistent customer footfall patterns.

---


## 📷 Dashboard Preview

![Coffee Shop Sales Dashboard](Coffee%20Shop%20Sales.png)
---

# 🚀 Outcome

This project helped strengthen skills in:

* Data Analysis
* Business Intelligence
* Dashboard Development
* KPI Tracking
* Data Visualization
* Business Insight Generation

---

# ⚙️ Data Cleaning & Transformation Process

The raw dataset was cleaned and transformed using Power Query in Excel before building the dashboard.

### Data Preparation Steps Performed

* Imported raw Excel dataset into Power Query for transformation.

* Created conditional columns to categorize product sizes into:

  * Small
  * Regular
  * Large
  * Not Defined

* Used Replace Values to standardize inconsistent size labels:

  * `Lg → Large`
  * `Sm → Small`
  * `Rg → Regular`

* Created a custom column to calculate total sales amount:

  `Total_Bill = Unit_Price * Transaction_Qty`

* Extracted transaction time from datetime column using:

  * Text After Delimiter

* Generated:

  * Month Name
  * Day Name

* Created proper weekday and month sorting using:

  * Day Number
  * Week Number
  * Month Number

* Used Power Pivot and Data Model for proper sequential sorting of weekdays and months.

---

# 📐 Measures & KPI Calculations

The following measures were created for KPI analysis:

### Total Sales

```DAX
SUM(Total_Bill)
```

### Total Footfall

```DAX
DISTINCTCOUNT(transaction_id)
```

### Average Bill Per Person

```DAX
SUM(Total_Bill) / DISTINCTCOUNT(transaction_id)
```

### Average Orders Per Person

```DAX
SUM(transaction_qty) / DISTINCTCOUNT(transaction_id)
```

### Top Selling Products

* Identified using sales revenue and quantity sold analysis.

---

# 📊 Dashboard Development

After data transformation and KPI creation:

* Pivot Tables were created for business analysis.
* Pivot Charts and visuals were developed.
* Interactive slicers were added for:

  * Month filtering
  * Day filtering
* KPI cards and business visuals were designed to provide actionable insights.

