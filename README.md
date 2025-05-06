# SQL E-Commerce Data Analysis

Collection of SQL queries to analyze performance of an e-commerce store.

## Objectives
- Analyze customer purchase behavior
- Inventory insights
- Monthly and regional sales trends

## Tools
- PostgreSQL / MySQL

## Example Query
```sql
SELECT customer_id, COUNT(order_id) AS total_orders, SUM(total_amount) AS total_spent
FROM orders
GROUP BY customer_id
ORDER BY total_spent DESC
LIMIT 10;
```
