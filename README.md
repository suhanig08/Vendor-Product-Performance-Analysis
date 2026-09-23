# Vendor & Product Performance Analysis

## Overview

This project analyzes vendor and product performance to understand **sales, procurement spend, profitability, purchasing efficiency, and inventory exposure**.

The analysis combines **SQL and Python-based data analysis** to identify high-performing vendors and products, evaluate procurement concentration, detect data-quality issues, and uncover opportunities for improving purchasing and commercial decisions.

## Objectives

- Identify vendors and products driving sales and procurement spend
- Evaluate vendor and product profitability
- Analyze procurement concentration across vendors
- Examine purchasing efficiency and sales-to-purchase relationships
- Identify products with low sales but strong margins and meaningful sales volume
- Analyze potential inventory exposure
- Compare profitability across different vendor performance groups

## Dataset

The dataset contains **10,692 records** and **18 attributes**, covering vendor, product, purchasing, sales, profitability and inventory-related information.

Key fields include:

- Vendor information
- Product and brand information
- Purchase price and quantity
- Sales price and quantity
- Purchase and sales values
- Gross profit
- Profit margin
- Stock turnover
- Sales-to-purchase ratio

## Tools & Technologies

- **SQL** – data extraction and querying
- **Python** – data analysis and processing
- **Pandas** – data manipulation and analysis
- **NumPy** – numerical computations
- **Matplotlib & Seaborn** – data visualization
- **SciPy** – statistical analysis
- **SQLite** – database querying

## Analysis Workflow

### 1. Data Extraction

The dataset is stored in a SQLite database and queried using SQL before being loaded into Python for further analysis.

```python
df = pd.read_sql_query(
    "SELECT * FROM vendor_sales_summary",
    conn
)
