# Superstore Sales \& Profitability Analysis

## Project Overview

This project focuses on analyzing Superstore sales data using **Microsoft Excel, Power Query, and Power BI**.

The objective was to transform raw sales data into an interactive business intelligence dashboard that provides a clear view of overall sales performance, profitability, orders, quantity, category performance, and sub-category performance.

The analysis combines data preparation, transformation, DAX calculations, KPI development, and interactive data visualization to support business performance analysis.

\---

## Key Performance Indicators

|KPI|Value|
|-|-:|
|Total Sales|$2.30M|
|Total Profit|$286.4K|
|Profit Margin|12.47%|
|Total Orders|5K|
|Total Quantity|38K|

\---

## Business Questions

The dashboard was developed to answer key business questions such as:

* What is the overall sales and profit performance?
* How do sales and profit change over time?
* Which product categories generate the highest sales?
* Which sub-categories contribute the most to profitability?
* Which sub-categories generate negative profit?
* How do sales, profit, and quantity compare across categories?
* How does performance vary across different regions and years?

\---

## Data Analysis Workflow

The project followed this workflow:

**Excel → Power Query → Power BI**

### 1\. Excel

The Superstore dataset was initially provided in Excel format and served as the source data for the analysis.

### 2\. Power Query

The dataset was imported into Power Query for data preparation and transformation.

The preparation process included:

* Reviewing the dataset structure
* Checking and correcting data types
* Preparing date fields for analysis
* Reviewing numerical fields
* Ensuring the dataset was structured appropriately for reporting

### 3\. Power BI

The transformed data was loaded into Power BI for data modeling, DAX calculations, and visualization.

A dedicated Date Table was created to support time-based analysis.

### 4\. DAX

DAX measures were created to calculate the key performance indicators used throughout the dashboard.

Some of the core measures include:

```DAX
Total Sales = SUM(Orders\[Sales])
```

```DAX
Total Profit = SUM(Orders\[Profit])
```

```DAX
Profit Margin = DIVIDE(\[Total Profit], \[Total Sales], 0)
```

```DAX
Total Quantity = SUM(Orders\[Quantity])
```

```DAX
Total Orders = DISTINCTCOUNT(Orders\[Order ID])
```

\---

## Dashboard Features

### KPI Overview

The dashboard provides a high-level view of:

* Total Sales
* Total Profit
* Profit Margin
* Total Orders
* Total Quantity

### Sales \& Profit Trend

A year-by-year comparison of sales and profit from **2014 to 2017**.

### Sales by Category

Sales performance is compared across:

* Technology
* Furniture
* Office Supplies

### Profit by Sub-Category

Profitability is analyzed across individual product sub-categories, highlighting both strong-performing and loss-making areas.

### Category Performance Analysis

Sales, profit, and quantity are compared across the major product categories.

### Interactive Filtering

Users can filter the dashboard by:

* Year
* Region
* Category

This allows different segments of the dataset to be explored interactively.

\---

## Key Findings

The analysis highlights several important patterns within the dataset:

* Total sales reached **$2.30M**, while total profit was **$286.4K**.
* The overall profit margin was **12.47%**.
* Technology recorded the highest sales among the three major categories.
* Profitability varied considerably across sub-categories.
* Some sub-categories generated negative profit, demonstrating that strong sales do not necessarily translate into positive profitability.
* Sales and profit increased across the later years of the analysis period, with **2017 recording the highest annual sales**.

These findings demonstrate why analyzing profitability alongside revenue is important when evaluating business performance.

\---

## Tools \& Technologies

|Tool|Purpose|
|-|-|
|**Microsoft Excel**|Data source and initial data handling|
|**Power Query**|Data transformation and preparation|
|**Power BI**|Data modeling and dashboard development|
|**DAX**|KPI and analytical measure calculations|

\---

## Skills Demonstrated

* Data Cleaning
* Data Transformation
* Power Query
* Data Modeling
* DAX
* KPI Development
* Business Intelligence
* Data Visualization
* Dashboard Design
* Business Performance Analysis

\---

## Project Structure

```text
Superstore-PowerBI-Analysis/
│
├── README.md
├── superstore.xlsx
├── dashboard-preview.png
├── dax-measures.md
└── SUPERSTORE DATASETS.pbix
```

\---

## Conclusion

This project demonstrates the process of taking raw business data from **Excel**, transforming it using **Power Query**, and developing an interactive **Power BI dashboard** to analyze sales and profitability.

The project focuses on turning raw transactional data into meaningful KPIs, trends, comparisons, and business insights that can support data-driven decision-making.

