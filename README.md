# E-commerce Database Management System

## 📌 Project Overview
This project is a relational database for a simple **E-commerce Store**.  
It manages customers, product categories, products, orders, and order items, with proper constraints and relationships.  

The database is designed in **MySQL** and can be run on **XAMPP** (phpMyAdmin/MySQL).  

---

## 🎯 Features
- **Customers**: Store customer details.
- **Product Categories**: Organize products into categories.
- **Products**: Store product details, stock, and pricing.
- **Orders**: Store customer orders with status tracking.
- **Order Items**: Manage many-to-many relationships between orders and products.

---

## 🛠️ Database Schema
- **One-to-Many**: Customer → Orders  
- **One-to-Many**: Category → Products  
- **Many-to-Many**: Orders ↔ Products (via Order Items)

---

## 📂 Files
- `ecommerce_db.sql` → Database creation script (schema + sample data).  

---

## 🚀 How to Run

### Option 1: Using phpMyAdmin
1. Start **XAMPP** (Apache + MySQL).  
2. Open [http://localhost/phpmyadmin](http://localhost/phpmyadmin).  
3. Click **Import**, choose `ecommerce_db.sql`, and click **Go**.  
4. Database `ecommerce_db` will be created with all tables and sample data.  

### Option 2: Using MySQL Command Line
```bash
mysql -u root -p < ecommerce_db.sql
