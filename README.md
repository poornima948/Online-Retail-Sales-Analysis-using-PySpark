# online-retail- sales-pyspark-analysis
 Online Retail Sales Analysis Using PySpark

This project performs an end-to-end analysis of the **UCI Online Retail dataset** using **PySpark** in **Google Colab**.  
It demonstrates data cleaning, transformation, feature engineering, and key business insights generation for a real-world e-commerce dataset.

---

 Dataset
- Original Dataset: [UCI Online Retail Dataset](https://archive.ics.uci.edu/ml/datasets/online+retail)
- [Download dataset](https://archive.ics.uci.edu/ml/machine-learning-databases/00352/Online%20Retail.xlsx)
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
  - Monthly Revenue Trend: total revenue generally increased towards the end of 2011, with the highest revenues in October and November, which aligns with holiday shopping trends.
  - Top Products by Quantity:
      1.PAPER CRAFT , LITTLE BIRDIE                       
      2. REGENCY CAKESTAND 3 TIER                           
      3. WHITE HANGING HEART T-LIGHT HOLDER               
      4. JUMBO BAG RED RETROSPOT                          
      5. MEDIUM CERAMIC TOP STORAGE JAR   
  - Top 5 Countries by Revenue :
      1. United Kingdom                 $7,285,024.64 | Customers: 3,920.0
      2. Netherlands                    $  285,446.34 | Customers:   9.0
      3. EIRE                           $  265,262.46 | Customers:   3.0
      4. Germany                        $  228,678.40 | Customers:  94.0
      5. France
  - Average Order Value
  - Revenue by Time of Day: Most orders were placed between 10 AM and 3 PM.
  - Top 20% Customers by Revenue Share

  Advanced Analysis:
  - Returned Product Detection
  - Country-wise Product Popularity
  - Small Order Frequency by Customer
  - Customer Contribution & Pareto Analysis
  - RFM Analysis & Customer Segmentation

---

 Sample Business Insights

- UK contributes over **80%** of total revenue. UK is by far the largest market,followed by the Netherlands and Germany. Also UK has most number of customers.
- Most revenue occurs during mid-day (10 AM – 3 PM)
- Top-selling products include **T-shirts** and **decor items**
- Most returns are associated with **low-cost**, bulk-ordered items
- Top 26% customers generate ~80% of total revenue

Monthly Revenue<img width="1377" height="664" alt="image" src="https://github.com/user-attachments/assets/47fe4d49-7818-4c04-b208-99f08ee9dc47" />

top 10 country revenue<img width="1372" height="671" alt="image" src="https://github.com/user-attachments/assets/351ee73b-d56d-4785-959c-2cbd1cb16bad" />

total quantity sold for top products<img width="1387" height="689" alt="image" src="https://github.com/user-attachments/assets/78e9a7f6-65d4-412d-a644-290a33464cd8" />

monthly average order value<img width="1388" height="686" alt="image" src="https://github.com/user-attachments/assets/2258be3e-ef12-4d91-9e00-16e53b38d7a3" />

top returned products<img width="1388" height="690" alt="image" src="https://github.com/user-attachments/assets/277bc727-e081-448f-8e82-a19cb7c2be09" />

---

## Analysis Summary 

Based on our analysis of the online retail data, we found the following:

**Customer Purchasing Behavior:**
- We calculated RFM metrics (Recency, Frequency, Monetary Value) for each customer, providing insights into their engagement and spending.

**Data Visualizations:**
- The time series plot of monthly total revenue showed peak revenue during the holiday season (October, November, and December).
- The bar chart of top countries by revenue indicated that the United Kingdom is the largest market.
- The bar chart of top products by quantity sold highlighted the most popular items.
- The time series plot of monthly average order value showed fluctuations throughout the year.

**Analysis of Returns:**
- We identified the top frequently returned products.
<img width="1189" height="590" alt="image" src="https://github.com/user-attachments/assets/bc663ebb-09e6-4ddc-b1cd-942085a9a981" />


**Segmentation based on RFM scores:**
<img width="669" height="212" alt="image" src="https://github.com/user-attachments/assets/4efc121d-c3e2-424b-8629-8d9ee5dc016c" />



This concludes our analysis .




---




