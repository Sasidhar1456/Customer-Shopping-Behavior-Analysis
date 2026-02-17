# 🛍️ Customer Shopping Behavior Analysis  

## 📌 Project Overview  

This project analyzes customer shopping behavior using **Python, SQL, and Power BI** to uncover revenue trends, customer segmentation patterns, and key business insights from **3,900+ transactions**.

The goal is to transform raw transactional data into actionable insights through data cleaning, statistical analysis, and interactive dashboards.

---

## 🚀 Tech Stack  

- **Python** (Pandas, NumPy, Matplotlib, Seaborn)
- **SQL** (Joins, Aggregations, Group By, Subqueries)
- **Power BI** (DAX, Data Modeling, Dashboard Creation)
- **Data Analysis & EDA**

---

## 📂 Dataset  

- Customer transaction data  
- 3,900+ records  
- Includes fields like:
  - Customer ID
  - Product Category
  - Purchase Amount
  - Payment Method
  - Date of Purchase
  - Gender / Age (if available)

---

## 🔎 Project Workflow  

### 1️⃣ Data Cleaning & Preprocessing (Python)
- Removed duplicates and null values  
- Standardized column formats  
- Converted date columns to proper datetime format  
- Validated data consistency  

### 2️⃣ SQL Analysis  
Wrote optimized SQL queries to:
- Calculate total revenue  
- Identify top-selling product categories  
- Analyze monthly revenue trends  
- Segment customers based on purchase behavior  
- Perform joins and aggregations for deeper insights  

Example:
```sql
SELECT 
    product_category,
    SUM(purchase_amount) AS total_revenue
FROM customer_transactions
GROUP BY product_category
ORDER BY total_revenue DESC;
```

---

### 3️⃣ Exploratory Data Analysis (Python)
- Revenue distribution analysis  
- Customer segmentation by age/gender  
- Trend analysis over time  
- Outlier detection  

Example:
```python
import pandas as pd

df = pd.read_csv("customer_shopping_behavior.csv")

# Total Revenue
total_revenue = df["Purchase Amount"].sum()
print("Total Revenue:", total_revenue)
```

---

### 4️⃣ Statistical Analysis
- Mean, Median, Standard Deviation  
- Revenue growth rate  
- Category-wise performance metrics  
- Customer spending patterns  

---

### 5️⃣ Power BI Dashboard
Created interactive dashboards with:

- 📊 Revenue KPI Cards  
- 📈 Monthly Sales Trend  
- 🛒 Category-wise Performance  
- 👥 Customer Segmentation  
- 💳 Payment Method Distribution  

Used **DAX measures** for:
- Total Revenue  
- Average Order Value  
- Revenue Growth %  
- Customer Count  

---

## 📊 Key Insights  

- Identified highest revenue-generating product categories  
- Discovered seasonal revenue patterns  
- Segmented customers based on spending behavior  
- Highlighted preferred payment methods  
- Revealed customer demographic trends  

---

## 💡 Business Impact  

- Helps in targeted marketing campaigns  
- Supports inventory planning  
- Improves customer retention strategies  
- Enables data-driven decision making  

---

## 📁 Project Structure  

```
Customer-Shopping-Behavior-Analysis/
│
├── data/
│   └── customer_shopping_behavior.csv
│
├── sql/
│   └── analysis_queries.sql
│
├── notebooks/
│   └── eda_analysis.ipynb
│
├── powerbi/
│   └── dashboard.pbix
│
└── README.md
```

---

## 🏁 Conclusion  

This project demonstrates end-to-end data analysis — from raw data cleaning to advanced dashboard visualization — using industry-standard tools.

It showcases practical skills in:
- SQL optimization  
- Data validation  
- Statistical analysis  
- Business intelligence reporting  
