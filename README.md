# Online Sales Data Analysis Project

This project performs a comprehensive **exploratory data analysis (EDA)** and **business intelligence (BI)** review of an online sales dataset.  
Using Python’s data science stack, the analysis extracts key performance indicators (KPIs), identifies sales trends, segments customer transactions, and pinpoints the most profitable products.

---

## Project Goals

The primary objectives of this analysis were to:

1. **Assess Overall Performance:** Calculate total revenue and total units sold.  
2. **Identify Top Performers:** Determine the most profitable product categories and individual products.  
3. **Analyze Trends:** Track revenue performance over time (monthly).  
4. **Understand Segmentation:** Analyze sales distribution by **Region** and preferred **Payment Method**.  
5. **Study High-Value Transactions:** Define and dissect transactions that contribute disproportionately to total revenue.  
6. **Evaluate Product Efficiency:** Explore the relationship between unit volume and revenue to identify high-ticket items.

---

## Technologies Used

- **Python 3**  
- **pandas** — Data manipulation and aggregation  
- **matplotlib** and **seaborn** — Data visualization  

---

## Key Findings & Visualizations

### 1. Overall Sales Performance
- **Total Units Sold:** The sum of all units sold across all transactions.  
- **Total Revenue:** The gross revenue generated across the entire dataset.

### 2. Product Revenue Drivers

The analysis segmented revenue by product category and individual product names to understand contributions.

| Analysis | Description | Visualization |
| :--- | :--- | :--- |
| **Top 5 Categories** | The top 5 product categories that contribute the highest total revenue. | Bar Chart |
| **Revenue Contribution** | A breakdown of total revenue share for each product category. | Pie Chart |
| **Top 10 Products** | The individual products generating the most cumulative revenue. | Bar Chart |

### 3. Sales Trends and Geographic Distribution
- **Monthly Total Revenue:** A line plot tracking revenue fluctuations across months to identify seasonal peaks and troughs.  
- **Transactions by Region:** A bar chart displaying transaction volume for **North America**, **Europe**, and **Asia**, showing comparative regional performance.

### 4. Pricing and Profitability

| Analysis | Description | Visualization |
| :--- | :--- | :--- |
| **Price Range** | Comparison of minimum and maximum unit prices within each product category, highlighting categories with wide pricing dispersion. | Box Plot |
| **Product Efficiency** | Scatter plot of total units sold vs. total revenue per product. The **Pearson correlation coefficient** was calculated as **0.87**, indicating a strong positive relationship. | Scatter Plot |
| **High-Ticket Items** | Products with **low units sold (≤ 2)** but **high total revenue (above 75th percentile)**, representing high-margin or premium items. | Filtered DataFrame |

### 5. Transaction Segmentation

#### High-Value Transactions
A **High-Value Transaction** is defined as one where total revenue exceeds the **75th percentile** of all transactions.  
- **Threshold:** \$5,200.45  
- **Distribution:** Bar charts visualize how these transactions are spread across **Regions** and **Product Categories**.

#### Payment Method Analysis
- **Most Popular Payment Method:** **Credit Card** identified as the most frequently used.  
- **Regional Reliance:** A cross-tabulation (`Region` vs `Payment Method`) revealed that **Europe** relies on **PayPal** for **61.5%** of its transactions.

