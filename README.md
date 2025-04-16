# Task6_Sql_-Sales-Trend-Analysis-Using-Aggregations-
🛍️ Project Title: Walmart Sales Data Analysis using SQL
📁 Overview:
This project involves the creation and analysis of a Walmart Sales database. It includes table creation, data cleaning, feature engineering (like time of day and day name), and data exploration using SQL queries.

🛠️ Key Steps & Components:
Database Creation

A database named walmartSales is created if it doesn't already exist.

Table Definition: sales

Fields include: invoice_id, branch, city, customer_type, gender, product_line, unit_price, quantity, tax_pct, total, date, time, payment, cogs, gross_margin_pct, gross_income, rating.

Data Cleaning

Initial queries select all data from sales for inspection.

Feature Engineering

time_of_day column is added using SQL CASE logic based on the time column:

Morning: 00:00:00 to 12:00:00

Afternoon: 12:01:00 to 16:00:00

Evening: Otherwise

day_name column is added using DAYNAME(date) function to extract the weekday.

Data Update Note

Notes are included to disable Safe Update Mode in MySQL Workbench before performing UPDATE queries.

Exploratory Analysis (in later parts of the script):

Likely includes aggregations, groupings by gender, payment method, product line, etc. (Based on common practice in similar projects)

📊 Purpose:
To transform raw transactional sales data into analyzable segments, helping in answering business questions like:

What time of day sees the most sales?

Which days have the highest sales?

What product lines are most popular?

