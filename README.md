# 📊 Project Title: Sales Performance Dashboard

An interactive Power BI dashboard designed to analyze sales performance, track targets, and identify business growth opportunities

## 📑 Table of Contents
* Project Overview
* Data Sources & Architecture
* Data Transformation (ETL)
* Data Model & DAX
* Dashboard Features
* Key Insights
* How To Use

---

## 🎯 Project Overview
Business Problem:
The organization needs a centralized solution to monitor sales performance, compare actual sales against targets, and identify high-performing regions and products.

Objective:
To provide actionable insights into sales trends, target achievement, profitability, and regional performance for better decision-making.

Target Audience:
Sales Managers, Business Analysts, Regional Managers, and Executive Leadership.



## 🗃️ Data Sources & Architecture
Source Systems:

- Microsoft Excel Sales Dataset
- Customer Data
- Product Data
- Sales Target Data

Data Volume:

- Approximately 10,000+ sales records
- Time Period: 2019–2022

Storage Mode:
Import Mode



## ⚙️ Data Transformation (ETL)
Tool Used:
Power Query Editor

Key Cleanups:

- Removed duplicate records
- Handled missing values
- Changed data types
- Merged sales and target tables
- Created date hierarchy
- Renamed columns for consistency

Custom Functions:
No custom M functions used.

---



## 🧠 Data Model & DAX
Model Type:
Star Schema

Fact Tables:

- Sales Fact

Dimension Tables:

- Date Dimension
- Product Dimension
- Customer Dimension
- Geography Dimension

Key Measures:

Total Sales = SUM(Sales[Sales])

Total Profit = SUM(Sales[Profit])

Total Orders = DISTINCTCOUNT(Sales[Order ID])

Sales Variance = [Total Sales] - [Total Target]

Achievement % = DIVIDE([Total Sales],[Total Target])*100
  ```

## 🖥️ Dashboard Features
Page 1: Sales Overview

- KPI Cards (Sales, Profit, Orders, Target Achievement)
- Monthly Sales Trend
- Sales by Category

Page 2: Sales Performance Analysis

- Actual vs Target Matrix
- Scatter Chart (Sales vs Profit)
- Performance by Category and Sub-Category

Page 3: Geographic Analysis

- Sales by City Map
- Order Count by State Funnel Chart
- Treemap for Sub-Category Sales Distribution

Design Theme:
Professional blue-themed dashboard with interactive slicers, drill-through functionality, and responsive visuals.

## 💡 Key Insights
Trend A:
Technology category generated the highest sales revenue across all categories.

Trend B:
Several regions achieved sales targets, while a few states showed significant sales variance.

Trend C:
A small number of sub-categories contributed a major share of total sales.

Recommendation:
Focus marketing efforts on high-performing categories and improve sales strategies in underperforming regions.



## 🚀 How To Use
1. Open the ".pbix" file in Power BI Desktop.
2. Refresh data using the Refresh button.
3. Use slicers to filter by year, category, or region.
4. Hover over visuals for detailed tooltips.
5. Analyze trends and performance metrics to support business decisions.



