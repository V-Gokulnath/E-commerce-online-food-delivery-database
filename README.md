# E-Commerce Online Food Delivery Database

## Project Overview
This project is designed using MySQL to manage an online food delivery system.  
It handles customers, restaurants, menu items, orders, payments, deliveries, and reviews efficiently.

---

## Features
- Customer Management
- Restaurant Management
- Menu Item Management
- Order Tracking
- Payment Handling
- Delivery Tracking
- Customer Reviews & Ratings

---

## Database Tables
- Customers
- Restaurants
- Menu_Items
- Orders
- Order_Items
- Payments
- Deliveries
- Delivery_Partners
- Reviews

---

## SQL Concepts Used
- DDL Commands
- DML Commands
- Joins
- Aggregate Functions
- Subqueries
- Views
- Stored Procedures
- Triggers
- Constraints
- Group By & Having

---

## Tools Used
- MySQL Workbench
- GitHub
- SQL

---

## Sample Queries

### Top Ordered Food Items
```sql
SELECT food_name, COUNT(*) AS total_orders
FROM Order_Items
GROUP BY food_name
ORDER BY total_orders DESC;
```

### Total Revenue
```sql
SELECT SUM(amount) AS total_revenue
FROM Payments;
```

### Customer Order Details
```sql
SELECT c.customer_name, o.order_id, o.order_status
FROM Customers c
JOIN Orders o
ON c.customer_id = o.customer_id;
```

---

## Project Objective
The main objective of this project is to design and manage a relational database for an online food delivery platform using SQL concepts.

---

## Author
**Gokulnath V**
