# E-Commerce-Sales-Analysis

## 📌 Overview

This project presents a comprehensive **data analysis pipeline** applied to the **Olist Brazilian E-Commerce Dataset**.
The goal is to integrate multiple relational datasets, engineer meaningful business metrics, and extract insights related to **sales performance, customer behavior, product categories, and geographic revenue distribution**.

The analysis is implemented using **Python**, leveraging **Pandas** and **NumPy** for efficient data manipulation and statistical computation.

---

## 🎯 Project Objectives

* 🔗 Consolidate multiple normalized e-commerce datasets
* 🧹 Perform data cleaning and datetime normalization
* 🛠️ Engineer revenue and time-based features
* 📊 Analyze sales trends and customer spending behavior
* 💾 Export analytical results for reporting and visualization

---

## 📂 Dataset Description

The project uses the following datasets from Olist:

* `olist_customers_dataset.csv`
* `olist_geolocation_dataset.csv`
* `olist_orders_dataset.csv`
* `olist_order_items_dataset.csv`
* `olist_order_payments_dataset.csv`
* `olist_order_reviews_dataset.csv`
* `olist_products_dataset.csv`
* `olist_sellers_dataset.csv`
* `product_category_name_translation.csv`

Each dataset represents a distinct component of the e-commerce transaction lifecycle.

---

## 🧰 Technologies Used

* 🐍 **Python 3.x**
* 🐼 **Pandas**
* 🔢 **NumPy**
* 📓 **Jupyter Notebook**

---

## 🔄 Data Processing Workflow

1. **📥 Data Ingestion**

   * Load all CSV files using Pandas
   * Inspect data types, structure, and missing values

2. **🧹 Data Cleaning**

   * Convert timestamp columns to `datetime`
   * Validate join keys and handle null values

3. **🔗 Data Integration**

   * Merge datasets using appropriate joins:

     * Orders ↔ Order Items
     * Products
     * Customers
     * Payments

4. **🛠️ Feature Engineering**

   * Total item value (`price + freight_value`)
   * Monthly order period extraction

5. **📊 Aggregation & Analysis**

   * Monthly revenue trends
   * Top-performing product categories
   * Revenue by customer state
   * Customer spend distribution statistics

6. **💾 Export Results**

   * Save curated outputs as CSV files

---

## 📈 Key Analyses Performed

* 📆 **Monthly Revenue Analysis**
* 🏷️ **Top 10 Product Categories by Revenue**
* 🗺️ **Revenue Distribution by Customer State**
* 👥 **Customer Spend Metrics**

  * Mean spend
  * Median spend
  * 90th percentile spend

---

## 📤 Generated Output Files

* `monthly_revenue.csv` – Monthly aggregated revenue
* `top_categories.csv` – Top 10 categories by total revenue
* `state_revenue.csv` – Revenue by customer state

---

## 🗂️ Project Structure

```text
.
├── data/
│   ├── olist_customers_dataset.csv
│   ├── olist_orders_dataset.csv
│   ├── olist_order_items_dataset.csv
│   └── ...
├── notebooks/
│   └── olist_sales_analysis.ipynb
├── outputs/
│   ├── monthly_revenue.csv
│   ├── top_categories.csv
│   └── state_revenue.csv
├── README.md
└── requirements.txt
```

---

## ▶️ How to Run the Project

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/olist-ecommerce-sales-analysis.git
   ```

2. Install dependencies:

   ```bash
   pip install pandas numpy
   ```

3. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

4. Run the notebook cells sequentially.

---

## 💼 Use Cases

* Exploratory Data Analysis (EDA)
* Business Intelligence prototyping
* Data analytics portfolio projects
* Revenue and customer behavior analysis
* Feature engineering practice for ML pipelines

---

## 🚀 Future Enhancements

* 📊 Data visualization (Matplotlib, Seaborn, Plotly)
* 👥 Customer segmentation (RFM analysis)
* 🚚 Delivery performance analysis
* 🤖 Predictive modeling and forecasting
* 📈 Dashboard integration (Power BI / Tableau)

---

## 📜 License & Credits

This project is intended for **educational and analytical purposes**.
All dataset rights and credits belong to **Olist** and the original data providers.

---
