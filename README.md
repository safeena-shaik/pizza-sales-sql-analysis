# 🍕 Pizza Sales SQL Analysis

## 📌 Project Overview

This project analyzes a year's worth of pizza sales data using **MySQL** to understand sales performance, customer ordering patterns, product popularity, and revenue contribution.

The project consists of **13 SQL business questions**, progressing from basic SQL analysis to more advanced concepts such as subqueries, window functions, ranking, percentage calculations, and cumulative revenue analysis.

The goal was to strengthen my ability to use SQL to transform raw sales data into meaningful business insights.

---

## 🎯 Project Objectives

The analysis aims to answer questions such as:

* How many orders were placed?
* How much revenue was generated?
* Which pizzas and sizes are most popular?
* Which pizza categories generate the most revenue?
* When are orders placed most frequently?
* Which pizzas are the top revenue generators?
* How does each pizza contribute to total revenue?
* How does revenue accumulate over time?
* Which pizzas perform best within each category?

---

## 🗂️ Dataset

The dataset contains four CSV files:

| File                | Description                                 |
| ------------------- | ------------------------------------------- |
| `orders.csv`        | Order date and time information             |
| `order_details.csv` | Pizza quantities associated with each order |
| `pizzas.csv`        | Pizza size and price information            |
| `pizza_types.csv`   | Pizza names, categories, and ingredients    |

### Dataset Period

**January 1, 2015 – December 31, 2015**

### Dataset Size

* **21,350 orders**
* **48,620 order-detail records**
* **96 pizza variations**
* **32 pizza types**

---

# 🛠️ Tools & Technologies

* **MySQL**
* **SQL**
* **CSV**
* **GitHub**

---

# 🔍 SQL Analysis

The queries are organized into three levels based on complexity.

## 🟢 Basic Analysis

The basic-level queries focus on fundamental SQL operations and overall sales metrics.

### Questions Answered

1. Retrieve the total number of orders placed.
2. Calculate the total revenue generated from pizza sales.
3. Identify the highest-priced pizza.
4. Identify the most common pizza size ordered.
5. List the top 5 most ordered pizza types along with their quantities.

### SQL Concepts

* `SELECT`
* `COUNT()`
* `SUM()`
* `MAX()`
* `GROUP BY`
* `ORDER BY`
* `LIMIT`
* `JOIN`

---

## 🟡 Intermediate Analysis

The intermediate-level queries explore sales patterns, pizza categories, and ordering behavior.

### Questions Answered

1. Find the total quantity of each pizza category ordered.
2. Determine the distribution of orders by hour of the day.
3. Find the category-wise distribution of pizzas.
4. Calculate the average number of pizzas ordered per day.
5. Determine the top 3 most ordered pizza types based on revenue.

### SQL Concepts

* `JOIN`
* Aggregate functions
* `GROUP BY`
* `ORDER BY`
* Date & time functions
* `AVG()`
* `SUM()`
* `COUNT()`
* Subqueries

---

## 🔴 Advanced Analysis

The advanced-level queries focus on revenue analysis and window functions.

### Questions Answered

1. Calculate the percentage contribution of each pizza type to total revenue.
2. Analyze the cumulative revenue generated over time.
3. Determine the top 3 pizza types based on revenue for each pizza category.

### SQL Concepts

* Window functions
* `RANK()`
* `SUM() OVER()`
* `PARTITION BY`
* Subqueries
* Percentage calculations
* Cumulative calculations
* Aggregate functions

### 🤖 AI-Assisted Learning

For the advanced-level analysis, I used **AI agents as a supporting learning resource** to better understand complex SQL concepts, particularly window functions, ranking, and cumulative calculations.

I reviewed, tested, and modified the queries against the dataset to understand the underlying SQL logic and validate the results.

---

# 📊 Key Findings

Some key findings from the analysis include:

* **Total Orders:** 21,350
* **Total Pizzas Sold:** 49,574
* **Total Revenue:** $817,860.05
* **Most Ordered Pizza Size:** Large
* **Highest-Priced Pizza:** The Greek Pizza — $35.95
* **Busiest Ordering Hour:** 12 PM
* **Average Pizzas Ordered Per Day:** 138.47

### Revenue by Category

| Category |     Revenue | Revenue Contribution |
| -------- | ----------: | -------------------: |
| Classic  | $220,053.10 |               26.91% |
| Supreme  | $208,197.00 |               25.46% |
| Chicken  | $195,919.50 |               23.96% |
| Veggie   | $193,690.45 |               23.68% |

### Top Pizza by Revenue

**The Thai Chicken Pizza — $43,434.25**

---

# 📁 Project Structure

```text
pizza-sales-sql-analysis/
│
├── data/
│   ├── orders.csv
│   ├── order_details.csv
│   ├── pizzas.csv
│   └── pizza_types.csv
│
├── sql/
│   │
│   ├── basic/
│   │   ├── 01_total_orders.sql
│   │   ├── 02_total_revenue.sql
│   │   ├── 03_highest_priced_pizza.sql
│   │   ├── 04_most_common_pizza_size.sql
│   │   └── 05_top_5_most_ordered_pizzas.sql
│   │
│   ├── intermediate/
│   │   ├── 06_quantity_by_pizza_category.sql
│   │   ├── 07_orders_by_hour.sql
│   │   ├── 08_pizza_category_distribution.sql
│   │   ├── 09_average_pizzas_per_day.sql
│   │   └── 10_top_3_pizzas_by_revenue.sql
│   │
│   └── advanced/
│       ├── 11_revenue_contribution_percentage.sql
│       ├── 12_cumulative_revenue_over_time.sql
│       └── 13_top_3_pizzas_by_revenue_per_category.sql
│
├── results/
│   └── Pizza_Sales_SQL_Results.pdf
│
└── README.md
```

---

# 📸 Query Results & Screenshots

The `results` folder contains screenshots of the SQL query outputs compiled into a PDF.

The results document provides a visual representation of the queries and their outputs, allowing the analysis to be reviewed without running the SQL scripts.

**Results PDF:**
`results/Pizza_Sales_SQL_Results.pdf`

> 📌 The results PDF will be added to this repository shortly.

---

# 💡 What I Learned

Through this project, I strengthened my understanding of:

* Writing SQL queries to answer business questions
* Working with multiple related tables
* Joining datasets using appropriate keys
* Aggregating and grouping sales data
* Working with dates and times
* Using subqueries
* Applying window functions
* Ranking records within categories
* Calculating percentage contributions
* Calculating cumulative revenue
* Translating business questions into SQL logic
* Using AI as a supporting tool while learning advanced SQL concepts

---

# 🚀 How to Run This Project

### 1. Clone the repository

```bash
git clone <your-github-repository-url>
```

### 2. Import the CSV files into MySQL

Load the four datasets from the `data` folder into your MySQL database.

### 3. Create the required tables

Create the corresponding tables for:

```text
orders
order_details
pizzas
pizza_types
```

### 4. Run the SQL queries

Navigate to the `sql` folder and run the queries according to their level:

```text
basic
intermediate
advanced
```

---

# 📌 Future Improvements

This project currently focuses on SQL-based analysis.

Planned improvements include:

* 📊 Creating an interactive **Power BI dashboard**
* 📈 Adding visualizations for key sales trends
* 🔎 Adding interactive filters for category, pizza size, and date
* 💼 Expanding the project into a complete end-to-end data analytics case study

---

# 👨‍💻 Author

**Shaik Mehaboob Safeena**

Aspiring Data Analyst | SQL | MySQL | Data Analytics

🔗 **LinkedIn:** https://www.linkedin.com/in/mehaboob-safeena-shaik-260117325/
