# 📚 Online Bookstore Sales Analysis (SQL + Power BI)

A data analytics project that explores sales performance, customer trends, and category insights for a mock online bookstore.

---

## 🔍 Project Overview
This project simulates a small online bookstore database with 4 key tables — `Customers`, `Books`, `Categories`, and `Sales`.

It demonstrates data analysis using **SQL** and interactive visualization with **Power BI**.

---

## 🧠 Objectives
- Analyze customer purchasing behavior
- Identify top-performing books and categories
- Evaluate city-wise and monthly sales performance
- Build an interactive Power BI dashboard for insights

---

## ⚙️ Tools & Skills Used
- **SQL** (Data Cleaning, Joins, Aggregations, Subqueries)
- **Power BI** (DAX, KPIs, Dashboards)
- **Data Modeling**
- **Git & GitHub**

---

## 📊 Dashboard Preview
![Dashboard Screenshot]([powerbi/dashboard_screenshot.png](https://1drv.ms/i/c/e424c45d39a8b00e/EcWg5qL1Gn9NiK-IMrZekaYB3XaTix4tlfcH5LoseztrRQ?e=OP7KNi)

---

## 🗂️ Dataset
The dataset includes 50+ sample entries for practice and visualization.

| Table | Description |
|--------|-------------|
| `Customers` | Customer demographics & cities |
| `Books` | Book titles, prices, and categories |
| `Sales` | Transaction data |
| `Categories` | Book genres |

---

## 💡 Key Insights
- Fiction and Technology categories lead total revenue.
- Age group **31–50** spends the most per order.
- Top cities: **New York, Los Angeles, Chicago.**
- Grace Lee and Eva Patel are the highest spenders.

---

## 🧾 SQL Queries
Check all analysis queries here: [`sql/analysis_queries.sql`]([sql/analysis_queries.sql](https://1drv.ms/t/c/e424c45d39a8b00e/EaefxG6B8PJNnlKIQSJqJn0B4A7hVOYUvKE6kctVf8dhXQ?e=B18kSZ))

Example:
```sql
SELECT City, SUM(Total_amount) AS City_Sales
FROM Customers c
JOIN Sales s ON c.Customer_id = s.Customer_id
GROUP BY City;
