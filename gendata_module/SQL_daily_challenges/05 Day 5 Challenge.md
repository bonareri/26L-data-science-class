## ABC_DATA – Nested Queries, CTEs & Window Functions Challenge

You are still the Data Analyst at ABC.

In this challenge, you must use:

- Nested queries (subqueries)
- Common Table Expressions (CTEs)
- Window functions

Do not solve everything using simple GROUP BY alone. The goal is to practice structured and layered querying.


## SECTION A – Nested Queries (Subqueries)

### 1. Orders Above Customer Average

Return orders where the order value is greater than the average order value for that same customer.

Show:
- order_id  
- customer_id  
- order_total  

### 2. Products Priced Above Category Average

Return products whose price is higher than the average price of all products.

Show:
- product_name  
- price  

Use a subquery in the WHERE clause.

### 3. Customers Who Spent More Than Overall Average

Return customers whose total spending is greater than the average total spending of all customers.

Show:
- customer_name  
- total_spent  

## SECTION B – Common Table Expressions (CTEs)

### 4. Revenue Per Product

Using a CTE:

Step 1: Calculate total revenue per product.  
Step 2: From that result, return products where total revenue is greater than 200.

Show:
- product_name  
- total_revenue  

### 5. Customer Order Summary

Using a CTE:

Step 1: Calculate number of orders per customer.  
Step 2: Return customers whose order count is above the average number of orders.

Show:
- customer_name  
- order_count  

### 6. Daily Revenue Report

Using a CTE:

Step 1: Calculate total revenue per order date.  
Step 2: Return all dates with their total revenue ordered from highest to lowest.

Show:
- order_date  
- daily_revenue  

## SECTION C – Window Functions

### 7. Rank Customers by Spending

Return:
- customer_name  
- total_spent  
- spending_rank  

Rank customers from highest to lowest spending.

### 8. Number Orders Per Customer

For each customer, number their orders in chronological order.

Show:
- customer_id  
- order_id  
- order_date  
- order_number  

Use ROW_NUMBER().

### 9. Running Total Revenue

Return:
- order_date  
- daily_revenue  
- running_total_revenue  

Use a window function to calculate the cumulative revenue over time.

## Bonus Challenge

Create one final query that returns:

- customer_name  
- total_orders  
- total_items  
- total_spent  
- spending_rank  

You must use:
- At least one CTE  
- At least one window function  
- At least one aggregate function  
