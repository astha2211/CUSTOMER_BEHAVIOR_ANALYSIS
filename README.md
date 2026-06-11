<div align="center">
  

  <h1>🛒 Customer Shopping Behavior Analysis</h1>
  <p><b>An end-to-end data analytics pipeline transforming raw consumer data into actionable retail insights.</b></p>

  <a href="https://python.org"><img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"></a>
  <a href="https://www.postgresql.org/"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL"></a>
  <a href="https://powerbi.microsoft.com/"><img src="https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI"></a>
  <a href="https://jupyter.org/"><img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white" alt="Jupyter"></a>

</div>

<br/>

## 📖 Overview

This project provides an end-to-end data analytics solution, transforming raw consumer data into actionable business insights. The pipeline covers the entire data lifecycle: from initial **Exploratory Data Analysis (EDA)** and cleaning in Python, to structured storage in **PostgreSQL**, and finally, interactive storytelling through a **Power BI** dashboard.

The goal is to analyze customer demographics and purchasing habits to identify trends that drive retail success.

---

## 📊 Dataset

The project utilizes the **Customer Shopping Preference Dataset**, containing over 3,900 detailed records. 

| Feature Category | Description |
| :--- | :--- |
| **Demographics** | Age, Gender, and Location across 50 US States. |
| **Transaction Details** | Item Purchased, Category, Purchase Amount (USD), and Payment Method. |
| **Customer Loyalty** | Subscription Status, Frequency of Purchases, and Promo Code usage. |
| **Feedback** | Review Ratings and Previous Purchase history. |

---

## 🛠️ Tools & Technologies

* **Language:** Python (Pandas, NumPy)
* **Database:** PostgreSQL (SQLAlchemy for ETL)
* **Visualization:** Power BI Desktop
* **Environment:** Jupyter Notebook

---

## ⚙️ Data Pipeline & Workflow

```mermaid
graph TD
    A[Raw CSV Data] -->|Pandas / NumPy| B(Python Jupyter Notebook)
    B -->|Clean & Transform EDA| C(Cleaned DataFrame)
    C -->|SQLAlchemy ETL| D[(PostgreSQL Database)]
    D -->|Direct Query| E[Power BI Desktop]
    E -->|Visual Analytics| F[Interactive Dashboard]
