# AdventureWorks Sales Analysis Dashboard (Power BI)

## 📊 Project Overview

This project is a **Power BI dashboard built using the AdventureWorksLT dataset**.
The goal of this report is to analyze product sales performance, category trends, and geographic distribution of sales.

The dashboard helps visualize how different products, categories, and regions contribute to overall sales.

---

## 🧾 Dataset

The dataset used in this project comes from **AdventureWorksLT**, a sample database provided by Microsoft.

Data Sources:

* AdventureWorksLT SQL Server database
* Additional US state codes dataset from Wikipedia (used for mapping)

Tables used:

* **Customers**
* **Sales**

---

## 🛠 Tools & Technologies

* **Power BI Desktop**
* **SQL Server**
* **Power Query (Data Transformation)**
* **DAX (Data Analysis Expressions)**

---

## 🔧 Data Preparation

Several transformations were applied before building the dashboard:

* Removed unnecessary columns
* Created a **LineTotal calculated column**
* Created a **Target Sales measure**
* Built relationships between tables
* Imported US state codes dataset
* Merged datasets to create a **State Code field** for geographic analysis

---

## 📈 Dashboard Visualizations

The dashboard contains the following visuals:

1. **Gauge Chart – Target Sales**

   * Shows current sales compared to target sales.

2. **Sales by Category (Bar Chart)**

   * Displays total order quantity by product category.
   * Includes a constant line benchmark.

3. **Top Selling Products (Column Chart)**

   * Highlights products generating the highest revenue.

4. **Top Selling Companies (Pie Chart)**

   * Shows which companies contribute most to sales.

5. **Sales by SubCategory (Donut Chart)**

   * Breaks down sales across product subcategories.

6. **Sales by State (Map Visual)**

   * Displays geographical sales distribution across US states.

---

## 📌 Key Insights

* **Bike category generates the highest sales volume.**
* A few companies contribute a large share of overall revenue.
* Certain products consistently outperform others in sales.
* Sales activity is concentrated in specific US states.

---

## 📷 Dashboard Preview

*(Add your dashboard screenshot here)*

Example:

```
![Dashboard Screenshot](dashboard.png)
```

---

## 💡 What I Learned

Through this project I practiced:

* Data modeling in Power BI
* Data cleaning using Power Query
* Creating calculated columns and measures
* Building interactive dashboards
* Visualizing geographic sales data

---

## 🚀 Future Improvements

Possible improvements for the dashboard:

* Add time-based sales analysis
* Include customer segmentation
* Create interactive filters and slicers
* Add KPI cards for quick metrics overview

---

## 👤 Author

**Ashadul Hasan**

Aspiring Data Analyst | Learning Data Analytics and Business Intelligence tools.

---
