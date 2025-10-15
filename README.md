# 🛒 E-Commerce Sales Analytics — PostgreSQL Project

![E-commerce SQL Project](https://img.shields.io/badge/E--Commerce-SQL%20Analytics-darkgreen?style=for-the-badge&logo=postgresql&logoColor=white)

---
![Banner Image](https://github.com/najirh/Amazon-Sales-Analysis-using-SQL-B4/blob/main/amazon.jpeg)
A comprehensive **PostgreSQL project** analyzing sales, revenue, inventory, and customer performance for an **E-commerce Business**.  
The project includes **20 advanced SQL business insights** and a **stored procedure** that automates inventory updates after every sale.

---

## 📁 Project Overview

This project demonstrates the use of **SQL for real-world business analysis** using normalized tables such as:
- `orders`
- `order_items`
- `products`
- `categories`
- `customers`
- `sellers`
- `inventory`
- `payments`
- `shipping`

Each query focuses on solving key **business challenges** like revenue tracking, sales trends, customer lifetime value, and inventory management.

---
## 🎯 Project Objectives

1. Collect and import data into PostgreSQL.  
2. Clean and transform data for consistency.  
3. Perform exploratory data analysis (EDA).  
4. Create optimized SQL queries and procedures.  
5. Generate insights and analytical reports.  
6. Conclude findings and suggest future improvements.

---

## ⚙️ Tech Stack

| Component | Description |
|------------|-------------|
| **Database** | PostgreSQL |
| **Language** | SQL (PL/pgSQL for procedure) |
| **Tools Used** | pgAdmin 4 / DBeaver / psql |
| **Concepts** | Joins, Aggregation, Window Functions, Subqueries, CTEs, Procedures, Ranking |

---

## 🧠 Key SQL Features Used

- `JOIN`, `GROUP BY`, `HAVING`, and `ORDER BY`
- `WINDOW FUNCTIONS` → `RANK()`, `DENSE_RANK()`, `LAG()`
- `CTEs (WITH)` for modular query design
- `CASE` expressions for conditional logic
- `Stored Procedures` using **PL/pgSQL**
- `DATE` and `INTERVAL` functions for trend analysis

---

## 📊 Business Problems Solved

| No | Business Query | Objective |
|----|----------------|------------|
| 1 | **Top Selling Products** | Identify top 10 products by total sales value. |
| 2 | **Revenue by Category** | Calculate total revenue and % contribution per category. |
| 3 | **Average Order Value (AOV)** | Find AOV for customers with >5 orders. |
| 4 | **Monthly Sales Trend** | Compare current vs last month sales trend. |
| 5 | **Customers with No Purchases** | Find registered users with zero orders. |
| 6 | **Best-Selling Categories by State** | Identify top categories per customer state. |
| 7 | **Customer Lifetime Value (CLTV)** | Rank customers by lifetime revenue. |
| 8 | **Inventory Stock Alerts** | Detect products with low stock levels. |
| 9 | **Shipping Delays** | Identify orders delayed beyond 7 days. |
| 10 | **Payment Success Rate** | Calculate percentage of successful payments. |
| 11 | **Top Performing Sellers** | Rank top 5 sellers with order success ratio. |
| 12 | **Product Profit Margin** | Compute and rank profit margins per product. |
| 13 | **Most Returned Products** | Show top 10 cancelled or returned items. |
| 15 | **Inactive Sellers** | Find sellers inactive for 6 months. |
| 16 | **Customer Return Behavior** | Classify customers as ‘Returning’ or ‘New’. |
| 17 | **Top 5 Customers by State** | Identify top 5 customers in each region. |
| 18 | **Revenue by Shipping Provider** | Calculate total and avg delivery time per provider. |
| 19 | **Revenue Decrease Ratio** | Detect top 10 products with YoY revenue drop. |
| 20 | **Stored Procedure - Inventory Update** | Auto-update inventory after each sale. |

---

## 🧩 Stored Procedure — `update_inventory`

The procedure automates **inventory management** after each sale:

```sql
CALL update_inventory(
    26002,    -- p_order_id
    2,        -- p_customer_id
    5,        -- p_seller_id
    26003,    -- p_order_item_id
    47,       -- p_product_id
    500       -- p_quantity
);
```

# Conclusion
Through this project, we aim to provide valuable insights into Amazon sales trends, customer preferences, and other factors influencing e-commerce operations.
By analyzing the dataset and addressing the key questions, we hope to assist stakeholders in making informed decisions
and optimizing their sales strategies. Feel free to explore the repository and contribute to further analysis or enhancements!
