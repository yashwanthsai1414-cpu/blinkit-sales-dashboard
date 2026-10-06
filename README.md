# Blinkit Sales Analysis Dashboard – Power BI

## Project Overview

This project analyzes Blinkit's grocery sales data using Power BI, SQL, Excel, Power Query, and DAX.

The objective is to identify sales trends, product performance, outlet performance, customer preferences, and key business KPIs.

## Tools & Technologies

- Power BI
- SQL
- Microsoft Excel
- Power Query
- DAX
- Data Cleaning
- Data Visualization

## Key KPIs

- Total Sales
- Average Sales
- Number of Items
- Average Rating
- Total Outlets
- Sales by Outlet Type
- Sales by Item Category
- Sales by Outlet Location
- Sales by Outlet Size

## Dashboard Analysis

### 1. Executive Dashboard

Provides an overview of:

- Total Sales
- Average Sales
- Total Items
- Average Rating
- Outlet Performance
- Sales Trends

### 2. Product Analysis

Analyzes:

- Item Categories
- Top Performing Products
- Low Performing Products
- Fat Content
- Average Sales by Category

### 3. Outlet Analysis

Analyzes:

- Outlet Type
- Outlet Size
- Outlet Location
- Outlet Establishment Year
- Sales Performance

## Data Cleaning

The dataset was cleaned using Power Query.

Major transformations included:

- Removing duplicate records
- Handling missing values
- Correcting data types
- Standardizing categorical fields
- Creating calculated columns
- Preparing data for Power BI modeling

## DAX Measures

```DAX
Total Sales =
SUM(Blinkit_Sales[Sales])

Average Sales =
AVERAGE(Blinkit_Sales[Sales])

Total Items =
COUNTROWS(Blinkit_Sales)

Average Rating =
AVERAGE(Blinkit_Sales[Rating])

Total Outlets =
DISTINCTCOUNT(Blinkit_Sales[Outlet_ID])
