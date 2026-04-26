🛍️ Online Retail Sales Analysis Using SQL

📌 Overview  
This project analyzes online retail sales data using SQL to understand business performance, customer purchasing patterns, and product trends through structured queries.

🎯 Objective  
To explore sales data and generate insights that help in tracking revenue, identifying top products, and understanding customer behavior.

 🛠️ Key SQL Concepts Used  
- SELECT, WHERE  
- GROUP BY, ORDER BY  
- Aggregate Functions (SUM, COUNT, AVG)  
- JOINS  
- Subqueries
   
 🧾 SQL Analysis
 🔹 Product-wise Sales Analysis
     SELECT product_name,
       SUM(sales) AS total_sales,
       SUM(profit) AS total_profit
FROM retail_sales
GROUP BY product_name
ORDER BY total_sales DESC;

 🔹 Monthly Sales Trend
 SELECT DATE_FORMAT(order_date, '%Y-%m') AS month,
       SUM(sales) AS total_sales
FROM retail_sales
GROUP BY month
ORDER BY month;

 🔹 Customer Purchase Analysis
 SELECT customer_id,
       COUNT(order_id) AS total_orders,
       SUM(sales) AS total_spent
FROM retail_sales
GROUP BY customer_id
ORDER BY total_spent DESC;
  
 🔍 Key Insights  
- Identified top-selling products generating highest revenue  
- Analyzed monthly sales trends and seasonal patterns  
- Observed customer purchasing behavior  
- Detected low-performing products for improvement  

 🧰 Tools Used  
- SQL  
- MySQL Workbench  
- Microsoft Excel  

📈 Business Impact  
- Helps in understanding revenue trends  
- Supports better product and sales strategy  
- Enables data-driven decision-making  

📌 Conclusion  
This project demonstrates how SQL can be used to analyze retail sales data and extract meaningful insights for business growth.
