# 🛒 Online Shopping Cart - DBMS Mini Project

📌 Project Overview

This project implements an Online Shopping Cart system using a relational database management approach. The primary goal is to simulate an e-commerce platform where users can:
- Search for products
- View product details and reviews
- Add or remove items from a cart using a drag-and-drop concept
  

 🧱 Features

- User-friendly product search and filtering
- Drag and drop interface simulation for cart management
- View and submit product reviews
- Payment handling with multiple modes
- AJAX-powered web interaction (conceptually described)

 🛠️ Tech Stack

- SQL – Core database creation, insertion, and querying

---

 📚 Database Design

 🔄 ER Diagram
> Present in the report (Page 9)

🗃️ Relational Schema Overview

| Table Name       | Description                           |
|------------------|---------------------------------------|
| `customer`       | Stores customer details               |
| `payment`        | Payment methods                       |
| `products`       | Product information                   |
| `admin`          | Admin who manages orders              |
| `onlinecart`     | Website/cart details                  |
| `p_category`     | Product categories and quantities     |
| `works_in`       | Admin and cart relationship           |
| `manages`        | Cart and product mapping              |
| `contains`       | Product and order relationship        |
| `makes`          | Customer payment and order mapping    |
| `visits`         | Customers visiting carts              |

---

 🧪 Sample SQL Queries
SELECT c.cname, s.p_id 
FROM customers c, products p, p_category s 
WHERE c.p_name = p.p_name AND p.p_id = s.p_id AND p_price = 1000;
