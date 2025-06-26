 Task 3: Writing Basic SELECT Queries

 Task Overview
This task demonstrates how to retrieve and filter data from the E-commerce database using basic SQL `SELECT` queries.

 Objective
* Extract data from one or more tables using `SELECT`
* Use conditions and filters with `WHERE`, `AND`, `OR`, `LIKE`, and `BETWEEN`
* Sort and limit results using `ORDER BY` and `LIMIT`

SQL Query Highlights

`SELECT *` and Specific Columns

sql
SELECT * FROM Products;
SELECT name, price FROM Products;
  Filtering with `WHERE`, `AND`, `OR`, `LIKE`, `BETWEEN`

sql
SELECT * FROM Customers
WHERE phone IS NOT NULL AND name LIKE 'A%';

SELECT * FROM Products
WHERE price BETWEEN 500 AND 50000;

SELECT * FROM Orders
WHERE order_date >= '2024-06-01' AND order_date <= '2024-06-30';

sql
SELECT * FROM Products
ORDER BY price DESC;

SELECT * FROM Customers
ORDER BY name ASC
LIMIT 2;
  Joins (Optional Advanced Step)

SELECT Orders.order_id, Customers.name, Orders.order_date
FROM Orders
JOIN Customers ON Orders.customer_id = Customers.customer_id;
 Outcome

* Efficient data extraction using `SELECT`
* Mastered common filtering, searching, and sorting techniques
* Built foundational querying skills for more advanced analytics


