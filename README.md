
# Maven Toys Sales Dashboard

This repository contains the Power BI dashboard created for Maven Toys, a fictitious chain of toy stores in Mexico. The dashboard provides comprehensive insights into sales, inventory, and store performance, aiding stakeholders in making informed decisions for business expansion.

## Table of Contents

- [Dataset](#Dataset)
- [Data Model](#data-model)
- [Visualizations](#visualizations)
- [Project Overview](#Project-Overview)
- [Creation process](#Creation-process)
- [Questions](#Questions)
- [Conclusion](#Conclusion)

## Dataset

The dataset includes sales and inventory data for Maven Toys, covering:
- Products
- Stores
- Daily sales transactions
- Current inventory levels

### Tables and Columns

- **Product**: `productid`, `productname`, `productcategory`, `productcost`, `productprice`
- **Stores**: `storeid`, `storename`, `storecity`, `storelocation`, `storesopendate`
- **Sales**: `date`, `storeid`, `productid`, `units`, `cost`, `price`, `revenue`, `profit`
- **Calendar**: `date`
- **Inventory**: `storeid`, `productid`, `stockonhand`

## Data Model

The data model follows a star schema, optimized for analytical queries:

- **Fact Table**: Sales, Inventory
- **Dimension Tables**: Product, Stores, Calendar

### Relationships

- Sales[productid] → Product[productid]
- Sales[storeid] → Stores[storeid]
- Sales[date] → Calendar[date]
- Inventory[productid] → Product[productid]
- Inventory[storeid] → Stores[storeid]


## Project Overview

Dataset Description
The dataset provided for this project includes comprehensive sales and inventory data from Maven Toys, a fictitious toy store chain operating in Mexico. It comprises daily sales transactions, product details, store information, and current inventory levels. The data is crucial for understanding the performance of various products and stores, identifying trends, and managing inventory efficiently.

Users of the Dashboard
The primary users of this dashboard are stakeholders and decision-makers at Maven Toys. This includes:

Executives: Interested in overall performance metrics such as revenue, profit, and growth rates.
Store Managers: Focused on store-specific data including sales, inventory levels, and store performance.
Sales and Marketing Teams: Looking to analyze product performance, sales trends, and campaign effectiveness.
Supply Chain Managers: Need insights into inventory levels, turnover rates, and stockout situations.

## Creation process

### Data Import and Preparation
I leveraged my expertise in data handling to import, clean, and transform the raw dataset using Power Query in Power BI. This involved extracting data from multiple Files, performing data cleansing operations, and shaping the data to fit the desired schema.

### Data Modeling
Using Power BI's data modeling capabilities, I constructed a star schema that optimized data relationships and facilitated efficient analytical queries. This involved defining fact and dimension tables, establishing relationships, and creating calculated columns and measures to enrich the dataset.

### Analysis with DAX
I applied my proficiency in Data Analysis Expressions (DAX) to derive valuable insights from the dataset. By writing complex DAX formulas, I calculated key performance indicators (KPIs), aggregated metrics, and performed advanced calculations to support decision-making processes.

### Data Visualization
Utilizing Power BI's robust visualization tools, I crafted compelling and intuitive visualizations to present insights effectively. From basic charts to interactive dashboards, I designed visually appealing representations of the data, making it easy for stakeholders to interpret and derive actionable insights.



## Questions
Addressed by the Dashboard
What are the total sales and profits?
Solution: KPI cards showing Total Revenue and Total Profit provide a quick overview of financial performance.

How have sales and profits trended over time?
Solution: Line charts displaying monthly trends in revenue and profit offer insights into performance over time.

Which products and stores are performing best?
Solution: Bar charts and pie charts show revenue by product category and by store, highlighting top performers.

What is the current inventory status?
Solution: Inventory tables and bar charts display current stock levels and inventory value by store, aiding in stock management.

How is the business growing compared to the previous month?
Solution: Cards showing month-over-month growth percentages provide a clear view of growth trends.

What is the gross margin and revenue growth rate?
Solution: Advanced measures calculate and display Gross Margin and Revenue Growth Rate, indicating profitability and growth.
By addressing these questions and problems, the dashboard empowers stakeholders to understand the business's current state, identify opportunities for improvement, and make strategic decisions for future growth.

## Conclusion
This dashboard provides a detailed analysis of sales and inventory data for Maven Toys, enabling stakeholders to identify trends, monitor performance, and make data-driven decisions. The use of various Power BI features, including DAX measures and interactive visualizations, ensures a comprehensive understanding of the business operations.
