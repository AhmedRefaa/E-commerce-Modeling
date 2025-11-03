E-commerce Sales Analysis Dashboard
A comprehensive e-commerce sales dashboard built with Power BI to analyze sales performance, customer behavior, and product trends from a CSV dataset.

Project Overview
This project involves the analysis of e-commerce sales data. The goal is to transform raw sales data into actionable insights using business intelligence tools. The core of this project is a Power BI report (ec_Data Modeling.pbix) that connects to a CSV data source (ec_data.csv) to visualize key performance indicators (KPIs) and trends.

This dashboard is designed to help business stakeholders (like sales managers, marketing teams, and executives) make data-driven decisions by providing a clear view of:

Overall sales performance

Product and category popularity

Geographical sales distribution

Payment method utilization and status

Dataset
The project uses a single flat-file data source:

File: ec_data.csv

Description: A transactional dataset containing detailed order information.

Key Columns:

Order ID

Date

Customer ID

Product Name

Category

Quantity

Total Sale Amount

Payment Method

Payment Status

Country

Continent

Tools & Technologies Used
This project relies on the Microsoft Power BI ecosystem:

Microsoft Power BI Desktop:

Use: The primary tool used for the entire project.

Functions:

Data Ingestion: Connecting to and importing the ec_data.csv file.

Data Modeling: Creating relationships, defining hierarchies, and building a robust data model (as indicated by the .pbix filename).

Data Visualization: Designing the interactive report, charts, tables, and maps.

DAX (Data Analysis Expressions): Writing custom formulas (measures and calculated columns) to derive insights not available in the raw data (e.g., Year-over-Year Sales, Total Pending Orders, etc.).

Power Query (M Language):

Use: Integrated within Power BI Desktop for ETL (Extract, Transform, Load).

Functions: Used to clean and transform the raw CSV data before loading it into the model. This could include changing data types, handling null values, or splitting columns.

DAX (Data Analysis Expressions):

Use: The formula language used inside Power BI.

Functions: Essential for creating the "brains" of the report. This project likely uses DAX to create key measures such as:

Total Sales

Total Orders

Average Order Value

Time-intelligence functions (e.g., SAMEPERIODLASTYEAR, DATESYTD)

Project Structure
/ec_data.csv: The raw, unprocessed e-commerce sales data.

/ec_Data Modeling.pbix: The complete Power BI project file. This file contains the data model, all data transformations (Power Query steps), all DAX measures, and the final report visualizations.

How to Use This Project
To explore this report:

Prerequisites: You must have Microsoft Power BI Desktop (a free application for Windows) installed on your computer.

Clone the Repository: Download or clone this repository to your local machine.

Bash

git clone [your-repository-url]
Open the Report: Navigate to the project folder and open the ec_Data Modeling.pbix file.

Update Data Source (If Necessary):

Power BI reports save the absolute path to their data sources. When you open the file on a new computer, it will likely show an error because it cannot find the ec_data.csv file at its original location.

To fix this:

In Power BI Desktop, go to the Home tab and click Transform data -> Data source settings.

Select the ec_data.csv source (it will have an error icon).

Click Change Source....

Click Browse and navigate to the ec_data.csv file in the folder you just cloned.

Click OK and then Close.

Click Refresh on the Home tab to load the data.

Potential Dashboard Features
(Based on the provided data, this report likely contains the following visualizations)

KPI Cards: Total Sales, Total Orders, Average Order Value.

Geographical Map: Sales by Country or Continent.

Bar Charts: Top 10 Products by Sales, Sales by Category.

Pie / Donut Charts: Order breakdown by Payment Status (Completed, Pending, Failed), Sales by Payment Method.

Line Chart: Sales trend over time (by Date).

Slicers: Interactive filters for Year, Continent, Category, and Payment Status.
