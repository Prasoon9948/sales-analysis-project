📊 Sales Insights Dashboard — Data Analytics Project
1. Project Overview

This project analyzes sales, customer, and product performance to help a business understand key patterns such as revenue trends, best-selling products, high-value customers, and profit margins.

It demonstrates a complete data analytics workflow:
Data Cleaning → SQL → Python EDA → Power BI Dashboard → Insights

2. Dataset Source

Dataset: Sales / Orders dataset (sample/Kaggle)
Contains:

Orders Table (OrderID, OrderDate, Sales, Quantity, Profit)

Customers Table (CustomerID, Name, Region, Segment)

Products Table (Category, Sub-Category, Price)

3. Tools Used

Python (Pandas, NumPy, Seaborn, Matplotlib)

SQL (joins, aggregations, grouping)

Power BI (DAX, dashboards, KPIs)

Excel

4. Data Cleaning & Preparation

Key steps completed in the Notebook:

Handle missing values

Fix date formats

Detect & remove duplicates

Engineer features (SalesAmount, ProfitMargin)

Clean categorical text values

5. SQL Analysis

Example SQL queries used:

🔹 Revenue by Category
SELECT Category, SUM(Sales) AS TotalRevenue
FROM Orders
GROUP BY Category
ORDER BY TotalRevenue DESC;

🔹 Top Customers
SELECT c.CustomerName, SUM(o.Sales) AS TotalSpent
FROM Orders o
JOIN Customers c ON o.CustomerID = c.CustomerID
GROUP BY c.CustomerName
ORDER BY TotalSpent DESC;

🔹 Monthly Sales Trend
SELECT DATE_FORMAT(OrderDate, '%Y-%m') AS Month,
       SUM(Sales) AS MonthlySales
FROM Orders
GROUP BY Month
ORDER BY Month;

6. Python EDA Notebook

Notebook includes:

Distribution analysis

Sales trends

Correlation heatmaps

Customer segmentation

Product profitability patterns

(Notebook file: Notebooks/sales_analysis.ipynb)

7. Power BI Dashboard

Dashboard includes:

Page 1 – Sales Overview

Total Sales

Total Profit

Profit Margin

Monthly & Yearly Trends

Page 2 – Product Insights

Top 10 products

Category performance

Discount impact

Page 3 – Customer Insights

Customer segmentation

High-value customers

Regional sales map

8. Key Findings

Technology category generates the highest revenue

15% of customers contribute 60%+ of total sales

Q3 and Q4 show seasonal sales spikes

High discounts reduce profitability in certain sub-categories

9. Project Files

📂 Data/ → CSV files

📂 Notebooks/ → Python EDA notebook

📂 SQL/ → SQL queries

📂 PowerBI/ → Dashboard files

10. Conclusion

This project demonstrates strong practical skills in:
✔ Data cleaning
✔ SQL analytics
✔ Python EDA
✔ Power BI dashboards
✔ Business insights generation

It represents a complete, job-ready Data Analyst project.
