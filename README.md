# 🛒 Zepto E-commerce SQL Data Analyst Project

## 📋 Project Overview
This is a complete, real-world data analyst portfolio project based on an e-commerce inventory dataset scraped from [Kaggle](https://www.kaggle.com/datasets/palvinder2006/zepto-inventory-dataset/data?select=zepto_v2.csv). This project simulates real analyst workflows, from raw data exploration to business-focused data analysis.

---

## 🛠️ Tech Stack & Tools
* **Role:** Data Analyst
* **Database Engine:** PostgreSQL
* **Interface:** pgAdmin 4
* **Dataset Source:** Scraped Zepto Inventory Data (CSV format)

---

## 🔧 Project Workflow

Here’s a step-by-step breakdown of what we do in this project:

### 1. Database & Table Creation
Started by creating a SQL table with appropriate data types.


### 2. Data Import
- Loaded CSV using pgAdmin's import feature.
  
- Faced encoding issues (UTF-8 error), which were fixed by saving the CSV file using CSV UTF-8 format.

### 3. 🔍 Data Exploration
- Counted the total number of records in the dataset

- Viewed a sample of the dataset to understand structure and content

- Checked for null values across all columns

- Identified distinct product categories available in the dataset

- Compared in-stock vs out-of-stock product counts

- Detected products present multiple times, representing different SKUs

### 4. 🧹 Data Cleaning
- Identified and removed rows where MRP or discounted selling price was zero

- Converted mrp and discountedSellingPrice from paise to rupees for consistency and readability
  
### 5. 📊 Business Insights
- Found top 10 best-value products based on discount percentage

- Identified high-MRP products that are currently out of stock

- Estimated potential revenue for each product category

- Filtered expensive products (MRP > ₹500) with minimal discount

- Ranked top 5 categories offering highest average discounts

- Calculated price per gram to identify value-for-money products

- Grouped products based on weight into Low, Medium, and Bulk categories

- Measured total inventory weight per product category
