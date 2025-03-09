# ETL-Driven Retail Analytics
Data Modeling for a Retail Store to Understand Consumer Behavior
Problem Statement
Retail businesses generate vast amounts of transaction data daily. However, without proper analysis, this data remains underutilized. The goal of this project is to model and analyze retail data to understand customer behavior, sales trends, and store performance. By leveraging SQL for ETL (Extract, Transform, Load) and analysis, we aim to provide insights into customer preferences, shopping patterns, and high-performing locations to help in data-driven decision-making.
________________________________________
Data Understanding
The dataset consists of multiple tables capturing different aspects of the retail business:
•	SALES_FACT: Transaction-level data, containing order details such as ORDER_ID, CUSTOMER_ID, STORE_ID, ORDER_DATE, and sales amounts.
•	CUSTOMER_INFO: Contains customer demographics, including CUSTOMER_ID, GENDER, AGE_GROUP, and LOYALTY_STATUS.
•	PRODUCT_INFO: Stores product details like PRODUCT_ID, PRODUCT_NAME, CATEGORY, and SALE_PRICE.
•	ORDER_PRODUCT_MAPPING: Maps ORDER_ID to multiple PRODUCT_IDs, capturing the quantity of each product purchased in a single order.
•	BRANCH_DETAILS: Contains information about store locations, including STORE_ID, CITY, AREA, and STATE.
________________________________________
Technology - ETL using SQL
The data pipeline involves an ETL process to extract, transform, and load data into a structured format:
1.	Extract: Data is fetched from different source tables (e.g., SALES_FACT, CUSTOMER_INFO).
2.	Transform: The data is cleaned, aggregated, and structured for analysis. This includes: 
o	Handling missing values
o	Standardizing formats
o	Creating derived columns (e.g., total_sales, customer_loyalty_segment)
3.	Load: The cleaned data is loaded into a structured database for querying and analysis.
SQL is used for all transformations and aggregations, ensuring data integrity and performance optimization.
________________________________________
Methodology
Aggregations
Aggregations help in summarizing data to extract key insights. Some examples:
•	Total Transactions by Gender: 
sql
CopyEdit
SELECT c.gender, COUNT(s.ORDER_ID) AS total_transactions
FROM SALES_FACT s
JOIN CUSTOMER_INFO c ON s.CUSTOMER_ID = c.CUSTOMER_ID
GROUP BY c.gender;
•	City with Highest Orders: 
sql
CopyEdit
SELECT b.city, COUNT(s.ORDER_ID) AS total_orders
FROM SALES_FACT s
JOIN BRANCH_DETAILS b ON s.STORE_ID = b.STORE_ID
GROUP BY b.city
ORDER BY total_orders DESC
LIMIT 1;
Joins
Joins are used to combine multiple tables for richer analysis. For example:
•	To calculate total sales per area: 
sql
CopyEdit
SELECT b.area, SUM(p.SALE_PRICE * op.QUANTITY_ORDERED) AS total_sales
FROM SALES_FACT s
JOIN ORDER_PRODUCT_MAPPING op ON s.ORDER_ID = op.ORDER_ID
JOIN PRODUCT_INFO p ON op.PRODUCT_ID = p.PRODUCT_ID
JOIN BRANCH_DETAILS b ON s.STORE_ID = b.STORE_ID
GROUP BY b.area
ORDER BY total_sales DESC
LIMIT 1;
This query joins four tables to get total sales per area, using a combination of inner joins and aggregations.
Creating Conditional Columns
To segment customers into loyalty tiers based on purchase frequency:
SELECT CUSTOMER_ID,
       CASE 
           WHEN COUNT(ORDER_ID) > 50 THEN 'High-Value'
           WHEN COUNT(ORDER_ID) BETWEEN 20 AND 50 THEN 'Medium-Value'
           ELSE 'Low-Value'
       END AS loyalty_segment
FROM SALES_FACT
GROUP BY CUSTOMER_ID;
This query categorizes customers into High-Value, Medium-Value, and Low-Value based on their purchase history.
________________________________________
Conclusion
Through data modeling and SQL-based ETL, we derived key insights into consumer behavior:
✅ Gender-based shopping trends – Identified how purchase frequency varies between men and women.
✅ Multi-store customers – Found customers shopping from more than one store.
✅ Top-performing locations – Identified cities and areas with the highest transactions and revenue.
✅ Customer segmentation – Classified customers into loyalty tiers based on their purchase frequency.
These insights help retailers optimize store operations, personalize marketing strategies, and improve customer retention. Future improvements include integrating machine learning models for predictive analytics and enhancing customer profiling.

