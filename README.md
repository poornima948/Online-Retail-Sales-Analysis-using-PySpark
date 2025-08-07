# online-retail-pyspark-analysis
 Online Retail Sales Analysis Using PySpark

This project performs an end-to-end analysis of the **UCI Online Retail dataset** using **PySpark** in **Google Colab**.  
It demonstrates data cleaning, transformation, feature engineering, and key business insights generation for a real-world e-commerce dataset.

---

 Dataset
- Original Dataset: [UCI Online Retail Dataset](https://archive.ics.uci.edu/ml/datasets/online+retail)
- Contains: ~500,000 transactions from a UK-based online store (December 2010 – December 2011)
- Due to GitHub's 25 MB upload limit, this project uses a **10,000-row sample** saved as `online_retail_sample.csv`  
   The sample was created using the first 10,000 valid rows from the original Excel file.

---

 Tools & Technologies

-  **PySpark** (DataFrame API)
-  **Seaborn** (for visualization)
-  **Matplotlib** (for visualization)
-  **Google Colab**
-  **pandas** (for initial Excel handling)
- `groupBy`, `agg`, `filter`, `when`, `withColumn`, and other PySpark transformations

---

 Business Goals

- Understand **total and monthly revenue** trends  
- Identify **top-selling products** and **high-value customers**  
- Find peak **order times** and **country-wise revenue**  
- Analyze **return rates** and low-value orders  
- Prepare insights for **data-driven business decisions**

---

Key Analysis Performed

 Data Cleaning: Removed rows with missing `CustomerID`, cancelled transactions, and negative quantities

 Feature Engineering:
  - `TotalPrice = Quantity × UnitPrice`
  - Extracted `Year`, `Month`, `Hour` from `InvoiceDate`

  KPI Metrics:
  - Monthly Revenue Trend
  - Top Products by Quantity
  - Top 5 Countries by Revenue
  - Average Order Value
  - Revenue by Time of Day
  - Top 20% Customers by Revenue Share

  Advanced Analysis:
  - Returned Product Detection
  - Country-wise Product Popularity
  - Small Order Frequency by Customer

---

 Sample Business Insights

- UK contributes over **80%** of total revenue
- Most revenue occurs during mid-day (10 AM – 3 PM)
- Top-selling products include **T-shirts** and **decor items**
- Most returns are associated with **low-cost**, bulk-ordered items
- Top 10% customers generate ~60% of total revenue

---




