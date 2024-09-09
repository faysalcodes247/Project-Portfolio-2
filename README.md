Global Mart Sales ETL Project

Project Overview

This project is an ETL (Extract, Transform, Load) process where I performed the role of a Data Engineer. The project focuses on extracting sales data from Kaggle, cleaning and transforming it using Python, and loading it into SQL for further analysis. The primary goal was to gain insights into Global Mart's sales performance through various analytical queries.

Project Workflow
1. Extract
The dataset was sourced from Kaggle (Global Mart Sales dataset).
Used Python's kaggle API to download and extract the required data.
File: orders.csv (containing sales data).
2. Transform
Cleaned the data by:
Handling missing values (e.g., treating 'Not Available', 'unknown' as NaN).
Renaming columns to follow a consistent naming convention (lowercase and underscores).
Derived new columns for additional insights, such as profit.
Converted order_date to the appropriate datetime format.
Removed unnecessary columns like list_price, cost_price, and discount_percent after transformation.
3. Load
The transformed data was loaded into a SQL database using SQLAlchemy.
Two methods were used:
Replacing the existing table.
Appending to the existing table if data already exists.
SQL Queries for Analysis
After loading the data into SQL, I performed the following analytical queries to extract business insights:

Top 10 Revenue-Generating Products: Identified the top products based on sales revenue.

Top 5 Products by Sales in Each Region: Used a Common Table Expression (CTE) to rank products by region.

Month-over-Month Sales Growth (2022 vs. 2023): Compared sales performance across the same months in different years.

Highest Sales by Month for Each Category: Determined which months had the highest sales for each product category.

Sub-category with the Highest Profit Growth (2022 vs. 2023): Found the sub-category with the highest year-over-year profit growth.

Tools and Technologies Used

Python: Data extraction, cleaning, and transformation.

SQLAlchemy: Loading data into SQL.

SQL (T-SQL): Data analysis and querying.

Kaggle API: Dataset extraction.

Pandas: Data manipulation and cleaning.

Jupyter Notebook: Development and documentation of the ETL process.

Installation & Setup


Future Enhancements

Automating the ETL pipeline using tools like Apache Airflow.
Extending the analysis to cover additional KPIs such as customer retention and cost analysis.
Implementing more advanced data transformations using Python and SQL.

Conclusion

This project demonstrates an end-to-end ETL process using real-world retail data. Through this process, I gained hands-on experience in data extraction, transformation, and loading, as well as advanced SQL querying for business insights.
