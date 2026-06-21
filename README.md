

@ -1 +1,59 @@
# PowerBI_readme-template
# PowerBI_readme-template

# 📊 Project Title: Sales Performance Dashboard

An interactive Power BI dashboard designed to analyze sales performance, track targets, and identify business growth opportunities.
## 📑 Table of Contents
*- Project Overview
- Data Sources & Architecture
- Data Transformation (ETL)
- Data Model & DAX
- Dashboard Features
- Key Insights
- How To Use

---

## 🎯 Project Overview
Business Problem

The company has sales data stored in multiple files, making it difficult to analyze overall business performance.

Objective

To clean, transform, merge, and model the data in Power BI and create a structured dataset for reporting and decision-making.

Target Audience

- Business Managers
- Sales Team
- Data Analysts
- Management Team

---

## 🗃️ Data Sources & Architecture
* Source Systems

- List of Orders.csv
- Order Details.csv
- Sales Target.csv

Data Volume

- List of Orders: First 500 records
- Order Details: Complete dataset
- Sales Target: Monthly target data

Storage Mode

Import Mode


## ⚙️ Data Transformation (ETL)
* **Tool Used:** Power Query Editor.
* **Key Cleanups:** List standard transformations applied to raw data (e.g., merging, unpivoting).
* **Custom Functions:** Mention any customized M code scripts used.

## 🧠 Data Model & DAX
Tool Used

Power Query Editor

Key Cleanups

- Imported CSV files
- Model Type:
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
* **Page 1: Overview:** High-level KPI cards and strategic macro trends.
* **Page 2: Deep Dive:** Interactive granularity with cross-filtering matrices.
* **Page 3: Performance:** Interactive drill-down features and customized tooltips.
* **Design Theme:** Highlight custom color palettes, JSON themes, or accessibility choices.

## 💡 Key Insights
Model Type

Star Schema

Fact Tables

- Order Details
- Orders Data

Dimension Tables

- List of Orders
- Sales Target

Key Measures

Total Amount = SUM('Orders Data'[Amount])

Total Profit = SUM('Orders Data'[Profit])

Profit Margin % = DIVIDE([Total Profit],[Total Amount],0)

---

🖥️ Dashboard Features

Page 1: Sales Overview

- Total Sales
- Total Profit
- Total Orders
- Profit Margin KPI Cards

Page 2: Category Analysis

- Average Profit by Category
- Total Amount by Sub-Category
- Interactive Filters

Page 3: Target Performance

- Monthly Sales Target
- Actual vs Target Comparison
- Drill-down Analysis

Design Theme

Simple business theme with interactive slicers and charts for easy analysis.

---

💡 Key Insights

Trend A

Sales performance varies across categories, with some categories generating higher profits than others.

Trend B

Profit Margin analysis identifies loss-making and break-even orders for better decision-making.

Recommendation

Focus on high-profit categories, reduce loss-making products, and monitor monthly targets regularly to improve overall business performance.

---



## 🚀 How To Use
1. Open the Power BI (.pbix) file in Power BI Desktop.
2. Refresh the data if the source files are updated.
