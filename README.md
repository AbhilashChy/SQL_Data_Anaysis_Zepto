🛒 Zepto E-commerce SQL Data Analyst Portfolio Project

A practical portfolio project built around an e-commerce inventory dataset scraped from Zepto, one of India’s fastest-growing quick-commerce startups. It mirrors real-world analyst workflows — from raw data handling to deriving actionable business insights.

📌 Project Summary

This project recreates how data analysts in the e-commerce industry use SQL to:

✅ Create and organize a real-world style e-commerce inventory database

✅ Run Exploratory Data Analysis (EDA) on product categories, stock, and pricing patterns

✅ Perform Data Cleaning to fix missing/invalid entries and convert prices from paise → rupees

✅ Build business-driven SQL queries to extract insights on pricing, stock, revenue, and more

📁 Dataset Details

Dataset originally scraped from Zepto product listings (sourced via Kaggle). It reflects real catalog complexity, where the same product may appear in multiple SKUs (different sizes, packaging, discounts, etc.).

Columns included:

sku_id: Unique product entry ID

name: Product name

category: Category (e.g., Fruits, Snacks, Beverages)

mrp: Maximum Retail Price (₹)

discountPercent: Discount applied

discountedSellingPrice: Final selling price (₹)

availableQuantity: Units in stock

weightInGms: Product weight in grams

outOfStock: Availability flag

quantity: Units per package

🔧 Workflow

1. Database Setup
Defined schema and created SQL table with appropriate data types.

2. Data Import
Loaded dataset using pgAdmin’s import feature (or \copy command for CSV import). Fixed UTF-8 encoding issues by saving as CSV UTF-8.

3. Data Exploration

Counted total records

Reviewed sample rows to understand data

Checked for null values

Listed unique product categories

Compared in-stock vs out-of-stock items

Detected duplicate product listings across SKUs

4. Data Cleaning

Removed invalid rows (zero MRP or price)

Standardized pricing (paise → rupees)

5. Business Analysis

Ranked Top 10 products by discount %

Found high-MRP products that are out of stock

Estimated category-wise revenue potential

Filtered premium products (MRP > ₹500) with minimal discounts

Ranked Top 5 categories by average discount

Analyzed price per gram to find best-value products

Classified products into Low / Medium / Bulk weight groups

Measured total inventory weight per category

🛠️ How to Use This Project
Clone the repository

git clone https://github.com/amlanmohanty/zepto-SQL-data-analysis-project.git
cd zepto-SQL-data-analysis-project
Open zepto_SQL_data_analysis.sql

This file contains:

Table creation

Data exploration

Data cleaning

SQL Business analysis

Load the dataset into pgAdmin or any other PostgreSQL client

Create a database and run the SQL file

Import the dataset (convert to UTF-8 if necessary)

Follow along with the YouTube video for full walkthrough. 👨‍💼
