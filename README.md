# Ecommerce_Sales-
SQL-based analysis of 10,000 e-commerce sales to explore customer trends, order status, delivery time, and cancellation insights.


# 🛒 E-Commerce Sales Analysis using SQL

A structured SQL project exploring online shopping behavior through synthetic data, built and analyzed to simulate real-world data analysis scenarios.

---

## ⭐ STAR Breakdown

### ✅ **Situation**
With the increasing volume of online transactions, businesses rely heavily on data analytics to improve operations and customer satisfaction. This project simulates an E-commerce company that wants to understand customer distribution, order patterns, delivery efficiency, and cancellation behavior using SQL-based insights.

### 🧾 **Task**
Build a realistic relational database with customer, order, product, and seller data and perform a wide range of SQL queries to answer business questions. The goal is to apply core SQL skills such as joins, aggregation, filtering, and grouping in a real-world structure.

### ⚙️ **Action**
- Created a synthetic dataset of 10,000 orders using Python and Faker.
- Designed a normalized relational schema with five tables:
  - `customers`, `orders`, `products`, `sellers`, and `geolocation`.
- Built the schema and constraints using MySQL Workbench.
- Created an Entity-Relationship (ER) diagram for structural clarity.
- Wrote and executed SQL queries at increasing difficulty levels:
  - 4 Easy: basic filters and counts
  - 3 Medium: aggregations, averages, and date formatting
  - 3 Hard: advanced joins, CASE statements, and logic-based filtering

### 📈 **Result**
- Developed 10 industry-style SQL queries covering customer behavior, delivery performance, cancellation trends, and product engagement.
- Demonstrated clear understanding of relational databases and query optimization.
- Gained hands-on experience with SQL that aligns with real-world data analyst responsibilities.

---

## 🗂️ Dataset Overview

| Table       | Description |
|-------------|-------------|
| `customers` | Contains customer ID and address details |
| `orders`    | Tracks purchases, delivery status, and dates |
| `products`  | List of products and their categories |
| `sellers`   | Seller info by location |
| `geolocation` | City and state mapped to zip codes |

---

## 🧩 Schema Design (ER Model)

```text
customers (customer_id) ───< orders (customer_id)
products  (product_id)  ───< orders (product_id)
sellers   (zip_code)    ───
customers (zip_code)    ─┬──> geolocation (zip_code)
sellers   (zip_code)    ─┘

## 📊 SQL Query Topics

### ✅ Easy
- **Customers by State**
- **Order Status Count**
- **Unique Products Sold**
- **Products by Category**

### ⚙️ Medium
- **Top States by Customers**
- **Average Delivery Time**
- **Monthly Order Count**

### 🔍 Hard
- **Top Ordering Customer**
- **Cancellation Rate by Category**
- **On-Time vs Delayed Orders**

---

## 💻 Tools Used

- **Python (Faker)** for data generation  
- **MySQL Workbench** for schema and queries  
- **SQL** for querying, aggregating, and analyzing  
- **PDF and CSV** formats for reporting and uploads

---

## 📁 Files Included

- `customers.csv`  
- `orders.csv`  
- `products.csv`  
- `sellers.csv`  
- `geolocation.csv`  
- `E-Commerce Sales.pdf` — slide-style summary
