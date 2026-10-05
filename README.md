# Olist E-Commerce Data Analytics Project

## 📌 Project Overview

This project focuses on analyzing e-commerce data from the Brazilian Olist marketplace using **PostgreSQL and Power BI**. The goal is to organize raw datasets into structured relational tables, prepare the data for analysis, and build an interactive dashboard to explore business performance and customer behavior.

The project demonstrates practical skills in SQL, relational database management, data modeling, and business intelligence visualization.

## 🎯 Project Objectives

* Import and organize the Olist e-commerce datasets into PostgreSQL.
* Create structured tables for customers, orders, products, sellers, payments, reviews, and geolocation data.
* Understand relationships between different datasets using common identifiers.
* Prepare data for reporting and visualization.
* Develop an interactive Power BI dashboard to explore e-commerce performance and business trends.

## 🛠️ Tools and Technologies

* **PostgreSQL** — Database creation, table definition, and data storage.
* **SQL** — Creating tables, defining primary keys, and structuring relational datasets.
* **Microsoft Power BI** — Data visualization and interactive dashboard development.
* **Kaggle** — Source of the Olist e-commerce dataset.

## 📂 Dataset Description

The project uses the Olist Brazilian E-Commerce Public Dataset, which contains information about orders, customers, products, sellers, payments, reviews, and delivery.

The data was divided into smaller fragments for importing into PostgreSQL.

The following nine datasets were structured as separate tables:

| Table Name                          | Description                                                  |
| ----------------------------------- | ------------------------------------------------------------ |
| `olist_customers_dataset`           | Customer identifiers, locations, and state information       |
| `olist_geolocation_dataset`         | Geographic coordinates and location information              |
| `olist_products_dataset`            | Product categories, dimensions, weight, and other attributes |
| `olist_sellers_dataset`             | Seller identifiers and location details                      |
| `olist_orders_dataset`              | Order status, purchase timestamps, and delivery dates        |
| `olist_order_items_dataset`         | Products purchased, sellers, prices, and freight charges     |
| `olist_order_payments_dataset`      | Payment methods, installments, and payment values            |
| `olist_order_reviews_dataset`       | Customer review scores, comments, and timestamps             |
| `product_category_name_translation` | Translation of product category names into English           |

## 🗄️ Database Design and SQL Implementation

PostgreSQL was used to create and organize the database tables before connecting the data to Power BI.

The SQL implementation includes:

* Creating tables with appropriate data types such as `TEXT`, `INTEGER`, `NUMERIC`, and `TIMESTAMP`.
* Defining primary keys for tables with unique identifiers.
* Storing geolocation data without a primary key because ZIP code prefixes can repeat.
* Using `DROP TABLE IF EXISTS ... CASCADE` to support recreating tables during development.
* Organizing related datasets using common identifiers such as `customer_id`, `order_id`, `product_id`, and `seller_id`.

These tables provide a foundation for connecting order transactions with customer, product, seller, payment, review, and delivery information.

## 📊 Power BI Dashboard

After importing the data into Power BI, an interactive dashboard was developed to present the data in a visual and business-friendly format.
The dashboard can serve as a foundation for exploring:

<img width="1322" height="742" alt="Screenshot 2026-10-05 213618" src="https://github.com/user-attachments/assets/5fd8b722-3d10-4b65-a41d-863cf0b5b33b" />
* **Overview – Executive Dashboard:**Provides a high-level view of overall business performance through key metrics and summary insights.
  
<img width="1326" height="741" alt="Screenshot 2026-10-05 213648" src="https://github.com/user-attachments/assets/ff9ff2c4-0e04-4955-a834-9c0b9200b14c" />
* **Sales Trend:** Analyzes sales performance and order trends over time to identify growth patterns and changes in business activity.

<img width="1323" height="742" alt="Screenshot 2026-10-05 213713" src="https://github.com/user-attachments/assets/48452282-c6e0-4f6f-84f3-14d9dab4591b" />
* **Category and Product:**Explores product categories and individual product performance to understand their contribution to overall sales.

<img width="1326" height="742" alt="Screenshot 2026-10-05 213732" src="https://github.com/user-attachments/assets/80fbd856-b52b-4a5c-9f9a-56b43e38fc01" />
* **Customer:** Examines customer distribution, purchasing behavior, and customer-related trends.

<img width="1152" height="645" alt="Screenshot 2026-10-05 213753" src="https://github.com/user-attachments/assets/8a3ece96-3220-4168-9c7d-7575e9ebf443" />
* **Delivery & Logistics:** Analyzes order delivery performance, shipping activity, and delivery timelines to evaluate operational efficiency..

*The specific metrics and insights depend on the visuals and measures implemented in the dashboard.*

## 🔄 Project Workflow

1. **Data Acquisition:** Downloaded the Olist dataset from Kaggle.
2. **Data Preparation:** Divided the dataset files into smaller fragments for importing.
3. **Database Setup:** Created the PostgreSQL tables using SQL scripts.
4. **Data Import:** Imported the dataset fragments into their respective tables.
5. **Data Connection:** Loaded the PostgreSQL data into Power BI.
6. **Dashboard Development:** Created visualizations and an interactive dashboard for exploring the e-commerce data.

## 💡 Key Learnings

* Working with a multi-table relational database.
* Writing SQL DDL statements to define database structures.
* Understanding relationships between transactional and reference datasets.
* Handling different data types, including timestamps and numerical values.
* Preparing structured data for Power BI reporting.
* Translating raw business data into interactive visualizations.


## 📚 Dataset Source

**Olist Brazilian E-Commerce Public Dataset — Kaggle**

Dataset link: https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce

The dataset contains anonymized information about orders placed through the Olist marketplace.

## 👨‍💻 Author

**Uday Tiwari**

Electronics and Communication Engineering undergraduate at IIIT Naya Raipur, interested in Data Analytics, SQL, Python, and business intelligence.
