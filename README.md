# 📦 Zepto SQL Data Analysis

A comprehensive SQL data analysis project performed on a retail dataset mimicking **Zepto’s** product inventory. This analysis includes **data exploration**, **data cleaning**, and **insightful business analysis** using SQL queries.

---

## 📂 Project Overview

This project simulates real-world SQL analytics on e-commerce product data, helping stakeholders make informed decisions based on:

- Stock availability
- Pricing and discount strategies
- Revenue forecasting
- Product categorization

---

## 📌 Objectives

- Explore and clean raw inventory data
- Perform SQL-based analysis to extract actionable insights
- Understand product-level and category-level metrics
- Group and segment products by pricing, weight, and availability

---

## 🧰 Technologies Used

- SQL (compatible with **PostgreSQL** / **MySQL**)
- Any SQL execution environment (e.g., DB Fiddle, MySQL Workbench, pgAdmin)

---

## 🧾 Dataset Schema

**Table Name:** `zepto`

| Column Name              | Data Type       | Description                                |
|--------------------------|------------------|--------------------------------------------|
| `sku_id`                 | SERIAL (PK)      | Unique product SKU                         |
| `category`               | VARCHAR(120)     | Product category                           |
| `name`                   | VARCHAR(150)     | Product name                               |
| `mrp`                    | NUMERIC(8,2)     | Maximum Retail Price in ₹                  |
| `discountPercent`        | NUMERIC(5,2)     | Discount percentage                        |
| `availableQuantity`      | INTEGER          | Quantity available in stock                |
| `discountedSellingPrice` | NUMERIC(8,2)     | Selling price after discount               |
| `weightInGms`            | INTEGER          | Product weight in grams                    |
| `outOfStock`             | BOOLEAN          | Indicates if product is out of stock       |
| `quantity`               | INTEGER          | Quantity shown to users (optional)         |

---

## 🔍 Data Exploration Highlights

- Row count and sample data
- Null value detection
- Unique categories listing
- In-stock vs Out-of-stock breakdown
- Detection of duplicate product names
- Products with invalid (zero) pricing

---

## 🧹 Data Cleaning

- Removed records with `MRP = 0`
- Converted prices from paise to rupees (divided by 100)
- Ensured price fields are clean and usable for analysis

---

## 📊 Analytical Queries & Insights

| Query | Description |
|-------|-------------|
| Q1 | Top 10 products with highest discount percentage |
| Q2 | High-MRP products that are currently out of stock |
| Q3 | Estimated revenue per category (selling price × stock) |
| Q4 | Products with MRP > ₹500 but low discount (<10%) |
| Q5 | Top 5 categories by average discount percentage |
| Q6 | Price per gram for products above 100g (value-based sorting) |
| Q7 | Group products by weight: Low (<1kg), Medium (<5kg), Bulk |
| Q8 | Total inventory weight per category |

---

## 💡 Business Use Cases

- 🔁 **Restocking Priority:** Detect high-value out-of-stock products.
- 🎯 **Targeted Discounts:** Optimize offers by comparing high/low discount categories.
- 📈 **Revenue Forecasting:** Estimate category-wise earnings potential.
- ⚖️ **Price Optimization:** Understand per gram pricing and value perception.
- 📦 **Inventory Planning:** Group products by weight to improve logistics.

---

## ▶️ How to Use

1. Clone the repo or download the `.sql` file.
2. Use any SQL platform like:
   - [https://www.db-fiddle.com](https://www.db-fiddle.com/)
   - MySQL Workbench / pgAdmin / SQLite Studio
3. Paste the queries step by step for exploration, cleaning, and analysis.
4. Modify or extend queries for your use case.

---

## 📜 License

This project is licensed under the **MIT License**.  
Feel free to use, modify, and share for educational or commercial purposes.

---

## 🙌 Acknowledgments

Inspired by Zepto’s real-world product data challenges.  
Developed as part of a **SQL data analytics portfolio project**.

