# 📊 E-Commerce Financial Analysis (TheLook Dataset)

## Overview

This project analyzes the **financial performance** of an e-commerce company using the **Google BigQuery public dataset: TheLook E-Commerce**. The analysis covers revenue, profitability, customer behavior, and geographic performance.

The workflow includes:

* SQL queries in BigQuery
* Data exploration and KPI calculations
* Connected Sheets integration for interactive analysis and scheduled refreshes
* Visualization in Looker Studio (Google Data Studio)
* Communicating insights with actionable recommendations

---

## Dataset

* **Source:** [`bigquery-public-data.thelook_ecommerce`](https://console.cloud.google.com/marketplace/details/bigquery-public-data/thelook-ecommerce)
* **Tables Used:**

  * `orders` – order metadata (order_id, user_id, created_at, status)
  * `order_items` – product-level order details (sale_price, quantity, status)
  * `products` – product information (category, name, cost)
  * `users` – customer demographics (name, country, email)

---

## Key Business Questions

1. How has **monthly revenue** trended over time?
2. Which **product categories** generate the most revenue and units sold?
3. What are the **most profitable products** by gross profit and margin?
4. Who are the **top customers** by lifetime value?
5. What percentage of customers are **repeat buyers**?
6. Which **countries** contribute most to revenue?

---

## SQL Highlights

* **Source:** [`SQL`](https://github.com/MoamenaSamir/E-Commerce-Financial-Analysis/blob/main/SQL)

* **Aggregations:** SUM, COUNT, AVG for financial KPIs
* **JOINS:** Combining orders, items, products, and users
* **GROUP BY + HAVING:** Filtering by profitable categories
* **CASE statements:** Customer segmentation by value
* **Temporary Tables & Views:** Created monthly revenue and rolling averages

---

## Dashboard

* **Tool:** Looker Studio
* **Link:** [View Dashboard](https://lookerstudio.google.com/reporting/3324c8ba-7f40-406b-9935-198848f2bba1)
* **Features:**

  * KPI cards (Revenue, Gross Profit, AOV, Gross Margin %)
  * Monthly revenue trend with rolling average
  * Top 10 customers by revenue
  * Revenue by country (map)
  * Revenue by product category
  * Top 20 products by gross profit

![Dashboard Screenshot][Dashboard](https://github.com/MoamenaSamir/E-Commerce-Financial-Analysis/blob/main/Dashboard.png)

---

## Insights

* **Total Revenue:** $8.1M
* **Gross Profit:** $4.2M (Gross Margin ~52%)
* **Top Category:** Outerwear & Coats (~$995K revenue)
* **Repeat Customers:** ~30% of customers made multiple purchases
* **Geography:** Highest revenue contributions from US, Canada, and parts of Europe/Asia

---

## Recommendations

1. Focus marketing and inventory on **top-performing categories** (Outerwear, Jeans, Sweaters).
2. Develop **loyalty campaigns** to increase repeat purchases.
3. Monitor **low-margin products** to optimize pricing strategy.

---

## Tools Used

* **SQL:** Google BigQuery
* **Spreadsheets:** Connected Sheets (Google Sheets)
* **Visualization:** Looker Studio (Google Data Studio)
* **Version Control:** GitHub

---

## Author

👤 [Moamena Samir]

* LinkedIn: [[My Profile](https://www.linkedin.com/in/moamena-samir-12b2a61b3/)]
---
