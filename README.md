# 📊 Retail Sales SQL Analysis — PostgreSQL

## 📌 Project Overview

This project performs **Retail Sales Data Analysis using PostgreSQL** to explore sales performance, customer behavior, product categories, and sales timing.

The analysis covers the complete SQL workflow, including:

- Creating a PostgreSQL table
- Importing data from CSV
- Data cleaning and standardization
- Filtering and sorting
- Aggregation and grouping
- Common Table Expressions (CTEs)
- Window functions
- `CASE WHEN` statements
- Customer and category analysis
- Business insights and recommendations

The dataset contains **2,000 retail transactions** covering **2022–2023**, with **155 unique customers** across three categories: **Clothing, Electronics, and Beauty**.

---

## 🎯 Project Objectives

The main objectives of this project are:

1. Build a clean, analysis-ready retail sales table.
2. Analyze revenue and order volume by product category.
3. Understand customer purchasing behavior.
4. Identify high-value transactions and top customers.
5. Analyze sales performance by month and year.
6. Understand sales patterns by time of day.
7. Generate actionable business insights from SQL analysis.

---

## 🗂️ Dataset

The dataset contains retail transaction information from **January 1, 2022 to December 31, 2023**.

### Main Columns

| Column | Description |
|---|---|
| `transaction_id` | Unique transaction ID |
| `sale_date` | Date of transaction |
| `sale_time` | Time of transaction |
| `customer_id` | Customer identifier |
| `gender` | Customer gender |
| `age` | Customer age |
| `category` | Product category |
| `price_per_unit` | Price per unit |
| `quantity` | Number of units sold |
| `cogs` | Cost of goods sold |
| `total_sale` | Total transaction value |

---

## 🛠️ Tools & Technologies

- **PostgreSQL**
- **SQL**
- CSV Dataset
- GitHub

---

## 🔄 Data Analysis Workflow

### 1. Table Creation & Data Import

A `retail_sales` table was created with appropriate PostgreSQL data types, followed by importing the CSV dataset using the `COPY` command.

### 2. Data Cleaning

The project checks for missing values across important columns and removes records containing NULL values.

Gender values were also standardized:

```sql
M → Male
F → Female
```



### 3. Business Analysis

The project answers **10 business questions** using SQL techniques such as:

- `WHERE`
- `GROUP BY`
- `SUM()`
- `COUNT()`
- `AVG()`
- `COUNT(DISTINCT)`
- `EXTRACT()`
- `RANK() OVER()`
- CTEs
- `CASE WHEN`

---

## ❓ Business Questions

### Q1. Sales on November 5, 2022

Retrieve all transactions made on **November 5, 2022**.

### Q2. Clothing Sales in November 2022

Identify Clothing transactions with higher quantities during November 2022.

### Q3. Revenue & Orders by Category

Calculate total revenue and number of orders for:

- Electronics
- Clothing
- Beauty

### Q4. Average Age of Beauty Customers

Find the average age of customers purchasing Beauty products.

### Q5. High-Value Transactions

Identify transactions where total sales exceeded **1,000**.

### Q6. Transactions by Gender & Category

Analyze transaction counts across gender and product categories.

### Q7. Monthly Sales Analysis

Calculate monthly sales for each year and identify the best-performing month.

### Q8. Top 5 Customers

Identify the top 5 customers based on total spending.

### Q9. Unique Customers by Category

Calculate the number of unique customers purchasing from each category.

### Q10. Orders by Time of Day

Categorize transactions into:

- 🌅 Morning
- ☀️ Afternoon
- 🌙 Evening

and analyze order volume by shift.

---

## 📈 Key Results & Insights

After data cleaning, the analysis contained **1,997 transactions** and generated total revenue of approximately **911,720**.

### Category Performance

| Category | Revenue | Orders |
|---|---:|---:|
| Electronics | 313,810 | 684 |
| Clothing | 311,070 | 701 |
| Beauty | 286,840 | 612 |

**Electronics** generated the highest revenue, while **Clothing** had the highest number of orders.

### Seasonal Sales Trend

**December** was the best-performing month in both years.

September–December generated approximately **57% of total revenue**, indicating a strong Q4 seasonal pattern.

### Customer Insights

The analysis identified the **top 5 customers by total spending**, with the highest customer spending approximately **38,440**.

### Time-of-Day Analysis

| Shift | Orders | Share |
|---|---:|---:|
| Evening | 1,062 | 53% |
| Morning | 558 | 28% |
| Afternoon | 377 | 19% |

Evening sales represent more than half of all orders, making evening a particularly important sales period.

---

## 💡 Business Recommendations

Based on the analysis:

1. **Prepare for Q4 demand**  
   Increase inventory, staffing, and promotional planning from September to December.

2. **Improve slow-month performance**  
   Introduce campaigns and offers during January–August to balance seasonal fluctuations.

3. **Focus on evening sales**  
   Since 53% of orders occur in the evening, consider evening promotions and targeted notifications.

4. **Reward high-value customers**  
   Introduce loyalty programs for customers with consistently high spending.

5. **Improve Beauty category performance**  
   Targeted promotions could help increase Beauty sales.

6. **Maintain broad marketing strategies**  
   Customer purchasing behavior is relatively balanced across genders.

---

## 🧠 SQL Skills Demonstrated

This project demonstrates practical SQL skills including:

- Database & table creation
- Primary keys
- PostgreSQL data types
- CSV data import
- Data cleaning
- NULL value handling
- Data standardization
- Filtering
- Sorting
- Aggregation
- `GROUP BY`
- `COUNT()`
- `SUM()`
- `AVG()`
- `COUNT(DISTINCT)`
- `EXTRACT()`
- `CASE WHEN`
- Common Table Expressions (CTEs)
- Window Functions
- `RANK() OVER(PARTITION BY...)`
- Business analysis and insight generation



---

## 📁 Project Files

```text
retail-sales-sql-analysis/
│
├── Retail_sales_sql_analysis.sql
├── SQL - Retail Sales Analysis.csv
├── Retail Sales SQL Analysis Project Report.pdf
└── README.md
```

### File Description

**`Retail_sales_sql_analysis.sql`**  
Contains the complete PostgreSQL SQL script, including table creation, data import, cleaning, and analysis queries.

**`SQL - Retail Sales Analysis.csv`**  
Raw retail sales dataset used for the analysis.

**`Retail Sales SQL Analysis Project Report.pdf`**  
Detailed project report containing methodology, results, business insights, recommendations, and conclusion.

---

## ⚠️ Project Notes

Before running the SQL script, the CSV file path in the `COPY` command should be updated according to your local PostgreSQL environment.

The project report also identifies a few script improvements, including the ranking direction in Q7 and the quantity condition in Q2.

---

## 🚀 Future Improvements

Possible extensions for this project include:

- Profit analysis using `total_sale - cogs`
- Month-over-month sales growth
- Customer segmentation
- Customer lifetime value analysis
- Category-level profitability
- Advanced sales trend analysis
- PostgreSQL views for reusable reporting

---

## 👨‍💻 Author

**Akash Rathore**

Aspiring Data Analyst | SQL | PostgreSQL | Excel | Power BI | Python

---

## ⭐ Conclusion

This project demonstrates how PostgreSQL can be used to transform raw retail transaction data into meaningful business insights.

The analysis highlights a relatively balanced performance across the three product categories, a strong September–December sales season, and a significant concentration of orders during evening hours.

This project is part of my **Data Analytics Portfolio** and demonstrates practical SQL skills applied to a real-world business analysis scenario.
