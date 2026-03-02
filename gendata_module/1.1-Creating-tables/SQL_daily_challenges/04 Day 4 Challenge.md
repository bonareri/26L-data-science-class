In this challenge, you will practice more advanced SQL queries, by nesting select queries and joining tables in the data. 

This a continuation of the previous day's challenge. Your task will be to answer the following questions:

### Which customer has made the most orders?

Hint, your query will have the following structure:

```sql
SELECT order_counts as (
    SELECT customer_id, count(order_id) AS order_count
    FROM xxxx
    GROUP BY xxxx
),
max_order_count AS (
    SELECT max(order_count) as max_count
    FROM xxxx
)
SELECT c.first_name, c.last_name
FROM xxxx c
JOIN order_counts oc ON c.customer_id = oc.customer_id
JOIN max_order_count moc ON oc.order_count = moc.max_count;
