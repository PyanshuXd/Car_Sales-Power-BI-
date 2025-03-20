# <div align="center">BMW Car Sales Dashboard</div>

![Intro]([https://github.com/PyanshuXd/Car_Sales-Power-BI-/blob/ee106da78926f70042efa697470090fa93295648/Images%20Used/1.png](https://github.com/PyanshuXd/Car_Sales-Power-BI-/blob/ee106da78926f70042efa697470090fa93295648/Images%20Used/man-woman-and-car-dealer-business-cartoon-concept-vector-11680254.jpg))

## Description:
This Power BI project provides an interactive dashboard for analyzing car sales data. It includes key insights such as total sales, revenue trends, top-selling models, and regional performance. The dashboard enables users to filter data dynamically, helping businesses make data-driven decisions.

## Problem Statement:
- The automotive industry generates vast amounts of sales data, which, if analyzed effectively, can provide valuable insights into sales performance, customer preferences, and market trends.
- This project aims to address the challenge of consolidating and visualizing BMW car sales data from Excel files to provide actionable insights for decision-making.

## Objectives:
- To consolidate BMW car sales data from multiple Excel files into a single Power BI dashboard.
- To create interactive visualizations that provide insights into sales performance, Top selling Models, Most expensive ones and Country & Channel wise sales.
- To enable stakeholders to make data-driven decisions by providing a clear and intuitive dashboard.

![Objective](https://github.com/PyanshuXd/Car_Sales-Power-BI-/blob/4d21e0d474381dba5af9f3daa155ac409863d1b7/Images%20Used/pngtree-car-salesman-in-dealer-showroom-image_77441.png)

## Technology Used in the Project:
- Power BI Desktop: For data modeling, visualization, and report creation.
- Microsoft Excel: For storing and managing raw data in three Excel files.
- Power Query: For data transformation and cleaning.
- DAX (Data Analysis Expressions): For creating calculated columns and measures.
- Power BI Service: For publishing and sharing the report online.

## Scope of the Project:
Consolidate data from three Excel files: Sales Data, Car Data, and Country Data.
- Create a relational data model to link the tables.
- Develop interactive visualizations to analyze sales trends, country wise performance, and customer demographics.
- Publish the report to Power BI Service for stakeholder access.

## Requirement Gathering for Visualization:
The following requirements were identified for the visualization:
- Sales Performance: Total sales, sales by region, and sales by car model.
- Product Analysis: Most Expensive sold car models and their profitability.
- Time-Based Analysis: Weekdays, Monthly and yearly sales trends.

![requirement]([https://github.com/PyanshuXd/SQL-Hospitality-/blob/84b1522911be548c834fba9fac83a5959606e58b/Images%20Used/hospital-management-system-fb.png](https://github.com/PyanshuXd/Car_Sales-Power-BI-/blob/622488da8d7f723d28b220dd07b41d37b83fce8b/Images%20Used/powerbi%20x%20excel.png))

## DAX Queries used and Execution Results:

•	Avg Price = DIVIDE([Revenue], [Qty Sold])
{This query shows the average price of model}

•	Qty Sold = SUM (factTable [Quantity Sold])
{This query shows the Quantity sold current year}

•	Qty Sold PY = CALCULATE ([Qty Sold], DATEADD('Calendar'[Date], -1, YEAR))
{This query shows the Quantity sold in previous year}

•	Revenue = SUM (factTable [Total])
{This query shows the Profit earned by specified model in current year}

•	Revenue PY = CALCULATE ([Revenue], DATEADD('Calendar'[Date], -1, YEAR))
{This query shows the Profit earned by specified model in current year}

•	Revenue Growth = DIVIDE ([Revenue Variance], [Revenue PY])
{This query shows the Revenue variance in Current year w.r.t Previous Year}

## Challenges Faced in the Project:
- Data Inconsistency: Some records in the Excel files had missing or inconsistent data, which required cleaning.
- Complex Relationships: Establishing relationships between multiple tables was initially challenging.
- Performance Issues: Large datasets caused slow loading times, which were resolved by optimizing the data model.

## Conclusion:
This Power BI project successfully consolidated and analyzed BMW car sales data from multiple Excel files, providing actionable insights through interactive visualizations. The dashboard enables stakeholders to make data-driven decisions, improving sales performance and customer satisfaction. With future enhancements, the project can further streamline sales analysis and forecasting.

## Screenshots:
Include screenshots of the Power BI dashboard, data model, and visualizations.

![Page 1](https://github.com/PyanshuXd/Car_Sales-Power-BI-/blob/d09efbc92f3a0edaa8bf5607ab7f485b6facfba3/Images%20Used/page1.png)
![Page 2](https://github.com/PyanshuXd/Car_Sales-Power-BI-/blob/d09efbc92f3a0edaa8bf5607ab7f485b6facfba3/Images%20Used/page2.png)
