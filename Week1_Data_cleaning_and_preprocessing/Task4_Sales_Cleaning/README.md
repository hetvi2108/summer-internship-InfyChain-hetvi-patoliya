# Superstore Sales Analysis

## Problem Statement
The Superstore dataset contains transactional sales data of a retail store.
The goal is to analyze business performance by identifying revenue trends,
top selling products, profit patterns and regional insights to derive
actionable business recommendations.

## Dataset
- **Source:** [Kaggle Superstore Dataset](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)
- **Rows:** 9994
- **Columns:** 21

## Approach

### 1. Data Cleaning
- Converted `Order Date` and `Ship Date` to datetime format
- Extracted `Month`, `Year` and `Month-Year` from Order Date
- Removed duplicates

### 2. Analysis Performed
- Monthly and yearly revenue trends
- Sales and profit analysis by category and sub-category
- Top 10 selling products by revenue
- Region wise sales and profit analysis
- Shipping method impact on profit for Tables and Bookcases
- Discount level impact on profitability

## Key Insights
- **Technology** is the most profitable category
- **Furniture** has high sales but the lowest profit margin
- **Tables and Bookcases** are the primary loss-making sub-categories
- **West** region performs best in both sales and profit
- **Central** region is the least efficient with lowest profit margin
- Discounts above **20%** are consistently associated with negative profitability
- Sales and profit both increased overall from **2014 to 2017**
- Sales peak every year between **September and December**

## Business Report
See [superstore_business_report.md](superstore_business_report.md)
for the complete business insights report with recommendations.

## Tools Used
- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook