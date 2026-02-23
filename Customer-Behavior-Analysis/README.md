# Customer Shopping Behavior Analysis

## 1. Project Overview

This project analyzes customer shopping behavior using transactional data from 3,900 purchases across various product categories. The goal is to uncover insights into spending patterns, customer segments, product preferences, and subscription behavior to guide strategic business decisions.

---

## 2. Dataset Summary

- Rows: 3,900  
- Columns: 18  

### Key Features:

- Customer demographics (Age, Gender, Location, Subscription Status)  
- Purchase details (Item Purchased, Category, Purchase Amount, Season, Size, Color)  
- Shopping behavior (Discount Applied, Promo Code Used, Previous Purchases, Frequency of Purchases, Review Rating, Shipping Type)  
- Missing Data: 37 values in Review Rating column  

---

## 3. Exploratory Data Analysis using Python

### Data Loading
Imported the dataset using pandas.

### Initial Exploration
Used df.info() to check structure and df.describe() for summary statistics.

---

### Missing Data Handling
Checked for null values and imputed missing values in the Review Rating column using the median rating of each product category.

---

### Column Standardization
Renamed columns to snake_case for better readability and documentation.

---

### Feature Engineering

- Created age_group column by binning customer ages  
- Created purchase_frequency_days column  
- Verified discount_applied and promo_code_used redundancy  
- Dropped promo_code_used  

---

### Database Integration
Connected Python script to PostgreSQL and loaded the cleaned DataFrame into the database for SQL analysis.

---

## 4. Data Analysis using SQL (Business Transactions)

- Revenue by Gender  
- Revenue by Category  
- Subscription vs Non-Subscription Analysis  
- Discount Impact Analysis  
- Top Rated Products  

---

## Tools Used

- Python (Pandas, Matplotlib, Seaborn)  
- SQL (PostgreSQL)  
- Power BI  
- GitHub
