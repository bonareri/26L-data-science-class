## ABC_DATA – Group By, CASE, Joins & Combined Queries Challenge

You are the Data Analyst at ABC.

Use the following concepts to answer the questions below:

- GROUP BY  
- HAVING  
- CASE WHEN  
- JOIN  
- Combined queries (UNION)

## SECTION A – GROUP BY & HAVING

### 1. Customers With High Spending

Return customers whose total spending is greater than 150.

Show:
- customer full name  
- total_spent  

Order the result from highest to lowest spending.

### 2. Top Selling Products

Return products that have been sold in total quantity greater than 5.

Show:
- product_name  
- total_quantity_sold  

### 3. Large Orders

Return orders where total quantity purchased is more than 4 items.

Show:
- order_id  
- total_items  

## SECTION B – CASE WHEN

### 4. Product Price Classification

Classify products as:

- Low - price < 30  
- Medium - price between 30 and 50  
- High - price > 50  

Return:
- product_name  
- price  
- price_category  

### 5. Customer Value Segment

Classify customers based on total spending:

- Gold - spending ≥ 200  
- Silver - spending between 100 and 199  
- Bronze - spending < 100  

Return:
- customer name  
- total_spent  
- segment  

## SECTION C – JOIN + GROUP BY

### 6. Product Revenue Summary

Return:
- product_name  
- total_quantity_sold  
- total_revenue  

### 7. Customer Purchase Overview

Return:
- customer name  
- number_of_orders  
- total_items_purchased  

## SECTION D – Combined Queries

### 8. Active vs Inactive Customers

Combine:

- Customers who placed at least one order labeled "Active"
- Customers who never placed an order labeled "Inactive"

Return:
- customer_name  
- status  

Use UNION.
