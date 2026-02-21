# Customer Shopping Behavior Analysis

## Overview

This project provides an end-to-end data analytics solution, transforming raw consumer data into actionable business insights. The pipeline covers the entire data lifecycle: from initial **Exploratory Data Analysis (EDA)** and cleaning in Python, to structured storage in **PostgreSQL**, and finally, interactive storytelling through a **Power BI** dashboard.

The goal is to analyze customer demographics and purchasing habits to identify trends that drive retail success.

---

## Dataset

The project utilizes the **Customer Shopping Preference Dataset**, containing 3,900 records. Key features include:

* **Demographics:** Age, Gender, and Location (50 US States).
* **Transaction Details:** Item Purchased, Category, Purchase Amount (USD), and Payment Method.
* **Customer Loyalty:** Subscription Status, Frequency of Purchases, and Promo Code usage.
* **Feedback:** Review Ratings and Previous Purchase history.

---

## Tools & Technologies

* **Language:** Python (Pandas, NumPy)
* **Database:** PostgreSQL (SQLAlchemy for ETL)
* **Visualization:** Power BI Desktop
* **Environment:** Jupyter Notebook

---

## Project Steps

### 1. Data Cleaning & EDA (Python)

* Handled missing values and verified data types.
* Performed statistical analysis to identify outliers in purchase amounts.
* Segmented customers by age groups and purchase frequency.

### 2. Database Integration (SQL)

* Established a connection between Python and PostgreSQL.
* **ETL Process:** Automated the loading of the cleaned DataFrame into a structured SQL table (`customer_behaviour`).
* Verified data integrity using SQL queries to ensure seamless reporting.

### 3. Visual Analytics (Power BI)

* Imported data directly from the PostgreSQL database.
* Designed a multi-page dashboard focusing on key performance indicators (KPIs).

---

## Dashboard Highlights

The interactive Power BI dashboard provides a deep dive into:

* **Sales Performance:** Total revenue segmented by Category and Season.
* **Customer Segmentation:** Identifying the most profitable age groups and genders.
* **Marketing Impact:** A comparison of purchase behavior between subscribed vs. non-subscribed customers.
* **Geographic Trends:** Mapping sales distribution across various US locations.

---

## Key Results

* **Category Insights:** Identified which product categories (e.g., Clothing, Footwear) drive the highest revenue.
* **Loyalty Analysis:** Quantified the impact of "Discount Applied" and "Subscription Status" on the average transaction value.
* **Operational Trends:** Discovered seasonal peaks in shopping behavior, providing a roadmap for inventory management.

---

## How It Runs

1. **Environment Setup:** Install dependencies using `pip install pandas sqlalchemy psycopg2`.
2. **Data Processing:** Run the Jupyter Notebook (`app.ipynb`) to clean the data and trigger the SQL export.
3. **Database:** Ensure PostgreSQL is running; the script will automatically create and populate the `customer` table.
4. **Visualization:** Open the `.pbix` file in Power BI and refresh the data source to view the latest insights.
