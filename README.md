# Power BI Dashboard --- Sales & Business Intelligence Analytics

## 📊 Overview

This Power BI dashboard provides an interactive business intelligence
view of an **electronics and mobile accessories business**. It presents
management-ready KPIs, sales and profit trends, product performance,
customer insights, regional analysis, payment methods, and profitability
analysis.

## 🎯 Business Objective

The dashboard helps management understand:

-   Overall sales and profit performance
-   Monthly sales and profit trends
-   Category and sub-category performance
-   Regional sales and profitability
-   Top and bottom performing products
-   Customer and order behavior
-   Payment method distribution
-   Profit-margin distribution
-   Discount impact on profitability

## 🛠️ Tools & Technologies

-   Power BI Desktop
-   DAX
-   Power Query
-   MySQL / SQL
-   Python
-   Pandas / NumPy
-   Matplotlib
-   CSV Dataset

## 📌 Dashboard Components

### Executive Dashboard

**KPI Cards** - Total Sales - Total Profit - Profit Margin - Total
Orders - Total Customers - Average Order Value (AOV)

**Visuals** - Monthly Sales & Profit Trend - Sales & Profit by
Category - Revenue Contribution by Category - Sales by Region - Profit
Margin Distribution - Sales by Payment Method - Top 10 Products - Bottom
10 Products - Sub-Category Performance

## 🎛️ Filters

The dashboard supports interactive filtering by:

-   Date Range
-   Category
-   Region
-   Customer Type

## 📈 Key DAX Measures

### Total Revenue

``` dax
Total Revenue = SUM(sales[sales])
```

### Total Profit

``` dax
Total Profit = SUM(sales[profit])
```

### Total Orders

``` dax
Total Orders = DISTINCTCOUNT(sales[order_id])
```

### Total Customers

``` dax
Total Customers = DISTINCTCOUNT(sales[customer_id])
```

### Total Units

``` dax
Total Units = SUM(sales[quantity])
```

### Average Order Value

``` dax
AOV = DIVIDE([Total Revenue], [Total Orders])
```

### Profit Margin

``` dax
Profit Margin = DIVIDE([Total Profit], [Total Revenue])
```

## 🔄 Data Flow

``` text
Raw Sales Data
      ↓
Python / Pandas
      ↓
Data Cleaning & Transformation
      ↓
Cleaned Sales Dataset
      ↓
SQL / MySQL Analysis
      ↓
Power BI Data Model
      ↓
DAX Measures
      ↓
Interactive Dashboard
      ↓
Business Insights & Recommendations
```

## 🧹 Data Preparation

The data preparation workflow includes:

-   Handling missing values
-   Removing duplicate records
-   Converting data types
-   Validating dates and numeric fields
-   Creating calculated columns
-   Creating profit-margin fields
-   Creating Year, Month, and Year-Month fields
-   Validating customer type
-   Checking KPI totals

## 👥 Advanced Analytics

The overall project also includes:

-   **RFM Analysis** --- Recency, Frequency, Monetary customer
    segmentation
-   **Cohort Analysis** --- customer retention and purchasing behavior
-   **Sales Forecasting** --- basic future sales direction analysis

## 💡 Business Questions Answered

1.  What are total revenue and profit?
2.  What is the overall profit margin?
3.  How many orders and customers are there?
4.  What is the average order value?
5.  Which categories generate the most revenue and profit?
6.  Which regions perform best?
7.  Which products are top and bottom performers?
8.  How are sales changing month by month?
9.  Which payment methods are most used?
10. Where are low-profit or loss-making transactions concentrated?
11. Which customer segments are most valuable?
12. Where can management improve profitability?

## 🚀 How to Open the Dashboard

1.  Clone or download this GitHub repository.
2.  Install **Power BI Desktop**.
3.  Open the `.pbix` report from the `dashboard/` folder.
4.  If prompted, update the dataset/source path.
5.  Click **Refresh**.
6.  Use the slicers to explore the dashboard.

> **Note:** The `.pbix` file is the actual Power BI report. The README
> only documents the dashboard. If the `.pbix` file is not included, the
> dashboard can be recreated using the cleaned dataset, DAX measures,
> and dashboard documentation.

## 📂 Recommended GitHub Structure

``` text
Sales-Business-Intelligence-Analytics/
├── data/
│   ├── raw/
│   └── cleaned/
├── notebooks/
│   └── sales_analysis.ipynb
├── sql/
│   ├── database_schema.sql
│   ├── data_analysis_queries.sql
│   └── business_queries.sql
├── dashboard/
│   ├── README.md
│   └── Sales_Business_Intelligence_Dashboard.pbix
├── reports/
│   ├── business_insights.md
│   ├── recommendations.md
│   └── kpis.json
├── visuals/
├── README.md
└── PROJECT_BRIEF.md
```

## 📸 Dashboard Preview

Place the dashboard screenshot inside the `dashboard/` folder as:

``` text
dashboard/dashboard_preview.png
```

Then add this to the GitHub README:

``` markdown
![Sales & Business Intelligence Dashboard](dashboard/dashboard_preview.png)
```

## 📌 Portfolio Skills Demonstrated

-   Business Intelligence
-   Power BI Dashboard Development
-   DAX
-   Power Query
-   Data Modeling
-   KPI Design
-   Sales Analytics
-   Customer Analytics
-   Product Analytics
-   Regional Analytics
-   Profitability Analysis
-   Business Storytelling

## 👨‍💻 Project Author

**Radhe Kant Raj**

**Project:** Sales & Business Intelligence Analytics\
**Domain:** Data Analytics / Business Intelligence\
**Tools:** Python \| SQL \| MySQL \| Power BI \| Pandas \| DAX

## ⭐ Conclusion

This dashboard transforms transaction-level sales data into an
interactive management reporting solution covering sales, profitability,
products, customers, regions, payment methods, and business performance.
