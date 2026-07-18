<!-- HEADER -->
<div align="center">
  <img src="https://images.unsplash.com/photo-1674027392887-751d6396b710?w=600&auto=format&fit=crop&q=60&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxzZWFyY2h8Nnx8ZSUyMGNvbW1lcmNlfGVufDB8fDB8fHwy" alt="Amazon Sales Banner" style="width:100%; max-width:800px; border-radius:12px;">
  
  <h1>🛒 Amazon Sale Report Analysis</h1>
  <p><strong>Unlocking Key E-Commerce Insights</strong></p>
  
  <p>
    <img src="https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python&logoColor=white" alt="Python">
    <img src="https://img.shields.io/badge/Pandas-2.0%2B-yellow?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas">
    <img src="https://img.shields.io/badge/Seaborn-0.12.0%2B-orange?style=for-the-badge&logo=python&logoColor=white" alt="Seaborn">
    <img src="https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge" alt="Status">
  </p>
  
  <p>
    <strong>Author:</strong> Imtiaz Ahmed &nbsp;|&nbsp;
    <a href="https://www.linkedin.com/in/imtiaz-ahmed-adar">
      <img src="https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat&logo=linkedin" alt="LinkedIn">
    </a>
  </p>
</div>

---

## 📖 Table of Contents

- [Project Overview](#-project-overview)
- [Key Business Questions](#-key-business-questions)
- [Technology & Tools](#-technology--tools)
- [Data Analysis & Insights](#-data-analysis--insights)
- [Visualizations](#-visualizations)
- [Project Structure](#-project-structure)
- [How to Run](#-how-to-run)
- [Future Work](#-future-work)
- [Connect with Me](#-connect-with-me)

---

## 📝 Project Overview

This project is a **comprehensive exploratory data analysis (EDA)** of Amazon sales data from a leading e-commerce platform in India. The goal was to transform raw transactional data into **actionable business intelligence** by examining revenue, order patterns, product performance, and customer behavior.

The analysis was conducted using **Python** within a Jupyter Notebook environment, leveraging powerful data science libraries like Pandas, Matplotlib, and Seaborn.

### 🎯 Key Business Questions Addressed

<details>
<summary><strong>Revenue Analysis</strong></summary>

- What was the total revenue generated from valid sales?
- How does revenue break down by status (e.g., valid, pending, cancelled, returned)?
- What are the monthly and quarterly revenue trends?
</details>

<details>
<summary><strong>Sales Performance</strong></summary>

- What is the distribution of order statuses?
- Which cities and states are the top revenue generators?
- What are the key sales channels and product categories driving revenue?
</details>

<details>
<summary><strong>Product Insights</strong></summary>

- Which product categories are the most popular?
- What is the distribution of product sizes?
- What is the revenue generated per unit and per order?
</details>

<details>
<summary><strong>Operational & Fulfillment</strong></summary>

- What percentage of orders are cancelled or returned?
- How do order counts vary by weekday and month?
- What is the revenue per order and per unit sold?
</details>

<details>
<summary><strong>Pareto Analysis</strong></summary>

- Which product categories contribute to the majority of the revenue (80/20 Rule)?
</details>

---

## 🧰 Technology & Tools

The following technologies and Python libraries were used to conduct this analysis:

<div align="center">

| Category | Tools & Libraries |
|----------|-------------------|
| **Data Manipulation** | Pandas, NumPy |
| **Data Visualization** | Matplotlib, Seaborn |
| **Development Environment** | Jupyter Notebook |

</div>

---

## 📊 Data Analysis & Insights

### 1. Data Preparation & Cleaning
The initial dataset contained **128,975 records** with several missing values and inconsistencies.

- **Data Cleaning**: Removed unnecessary columns (e.g., `index`, `Courier Status`, `Unnamed: 22`).
- **Handling Missing Values**: Filled missing values in `ship-state` and `ship-city` with 'unknown', and missing `Amount` values with 0 after analyzing their association with `Status`.
- **Data Type Conversion**: Converted the `Date` column to a `datetime` object and formatted categorical columns (e.g., `month`, `weekday`, `Size`) for better analysis.
- **Data Correction**: Standardized state names for consistency.

### 2. Key Financial Metrics
The analysis revealed critical financial insights:

| Metric | Value |
|--------|-------|
| **Total Revenue** | **$696,632.93** |
| **Revenue Per Unit Sold** | **$6.60** |
| **Revenue Per Order** | **$6.63** |
| **Revenue from Valid Sales** | **$696,632.93** |
| **Pending Orders Amount** | **$6,224.09** |
| **Cancelled Orders Amount** | **$69,192.84** |
| **Returned Orders Amount** | **$13,876.92** |

### 3. Temporal Trends
Analyzing the data over time provided key patterns:

<table>
<tr>
<th>Metric</th>
<th>Insight</th>
</tr>
<tr>
<td><strong>Sales Channels</strong></td>
<td>The "Amazon.in" channel dominated with <strong>99.90%</strong> of sales.</td>
</tr>
<tr>
<td><strong>Top Month</strong></td>
<td><strong>April</strong> was the highest-performing month with <strong>$256,688.48</strong> in revenue.</td>
</tr>
<tr>
<td><strong>Quarterly Revenue</strong></td>
<td>Q2 (April-June) generated <strong>$695,691.10</strong> vs. Q1 (March) <strong>$941.83</strong>.</td>
</tr>
<tr>
<td><strong>Peak Day</strong></td>
<td><strong>Sunday</strong> was the top day for orders.</td>
</tr>
<tr>
<td><strong>Growth Rate</strong></td>
<td>March to April: <strong>27,154.23%</strong> growth, followed by a decline in May and June.</td>
</tr>
</table>

### 4. Product & Category Performance
The analysis of product data offered insights into customer preferences:

- **Top Product Sizes**: **M, L, and XL** were the most popular sizes.
- **Pareto Analysis**: The **"Set"** and **"Kurta"** categories together accounted for over **77%** of total revenue, representing a classic 80/20 rule.

### 5. Geographic Insights
Customer location data was a major focal point for understanding market penetration:

<table>
<tr>
<th>Top Cities</th>
<th>Revenue</th>
<th>Top States</th>
<th>Revenue</th>
</tr>
<tr>
<td>Bengaluru</td>
<td>$65,854.77</td>
<td>Maharashtra</td>
<td>$119,554.92</td>
</tr>
<tr>
<td>Hyderabad</td>
<td>$49,481.95</td>
<td>Karnataka</td>
<td>$94,362.23</td>
</tr>
<tr>
<td>Mumbai</td>
<td>$38,901.75</td>
<td>Telangana</td>
<td>$61,237.78</td>
</tr>
</table>

### 6. Operational Fulfillment
Analyzing order statuses and volume helped assess operational health:

| Order Status | Count |
|--------------|-------|
| **Shipped** | 77,804 |
| **Shipped - Delivered to Buyer** | 28,769 |
| **Cancelled** | 18,332 |
| **Shipped - Returned to Seller** | 1,953 |
| **Pending** | 658 |

- **Cancellation Rate**: **14.21%** (Acceptable for a platform like Amazon)
- **Return Rate**: **1.64%** (Indicating good product quality)

---

## 📈 Visualizations

The analysis utilized a variety of high-quality visualizations to effectively communicate key findings:

### Financial Overview
- Financial Overview Summary (Revenue, Pending, Cancelled, Returned)
- Revenue Outliers Detection

### Temporal Visualizations
- Monthly Revenue Trend
- Monthly Orders vs. Cancelled Orders Summary
- Growth Percentages Over Months
- Orders by Weekday

### Product & Category Visualizations
- Size Distribution
- Pareto Chart of Revenue by Category

### Geographic Visualizations
- Top 10 Revenue Generated Cities
- Top 10 Revenue Generated States

### Operational Visualizations
- Orders Quantity Distribution
- Orders Quantity vs Orders Amount