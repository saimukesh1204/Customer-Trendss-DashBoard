# 🛍️ Customer Shopping Behavior Analysis

## 📌 Overview
This project delivers a comprehensive analysis of **customer shopping behavior** using transactional data from **3,900 purchases** across multiple product categories.  
The objective is to uncover **spending patterns, customer segments, product preferences, and subscription behavior** to support **data-driven business decisions**.

---

## 📊 Dataset Summary
- **Rows:** 3,900  
- **Columns:** 18  
- **Key Features:**
  - Customer demographics → Age, Gender, Location, Subscription Status  
  - Purchase details → Item Purchased, Category, Purchase Amount, Season, Size, Color  
  - Shopping behavior → Discount Applied, Promo Code Used, Previous Purchases, Frequency of Purchases, Review Rating, Shipping Type  
- **Missing Data:** 37 values in *Review Rating* column

---

## 🐍 Exploratory Data Analysis (Python)
- Data loading and cleaning with **pandas**  
- Summary statistics using `.info()` and `.describe()`  
- Missing data imputation (median rating per product category)  
- Column standardization (snake_case naming convention)  
- Feature engineering:
  - `age_group` (binned ages)  
  - `purchase_frequency_days` (derived from purchase history)  
- Redundancy check → dropped `promo_code_used`  
- Integrated cleaned dataset into **PostgreSQL** for SQL analysis

---

## 🗄️ SQL Business Insights
Structured queries in MySQL revealed key findings:

- **Revenue by Gender** → Male customers generated higher revenue than female customers  
- **High-Spending Discount Users** → Customers using discounts but spending above average  
- **Top Products by Rating** → Gloves, Sandals, Boots, Hat, Skirt  
- **Shipping Type Comparison** → Express shipping customers spent slightly more than Standard  
- **Subscribers vs. Non-Subscribers** → Non-subscribers contributed more total revenue, but subscribers had similar average spend  
- **Discount-Dependent Products** → Hat, Sneakers, Coat, Sweater, Pants had highest discount usage  
- **Customer Segmentation** → Loyal (3,116), Returning (701), New (83)  
- **Top Products per Category** → Blouse, Pants, Shirt (Clothing); Jewelry, Sunglasses, Belt (Accessories)  
- **Repeat Buyers & Subscriptions** → Repeat buyers more likely to subscribe  
- **Revenue by Age Group** → Young Adults contributed the highest revenue

---

## 📈 Power BI Dashboard
An interactive dashboard was developed in **Power BI** to visualize:
- Total Customers → **3.9K**  
- Average Purchase Amount → **$59.76**  
- Average Review Rating → **3.75**  
- Revenue & Sales by Category  
- Subscription Status distribution  
- Revenue & Sales by Age Group  
- Shipping Type preferences  

---

## 💡 Business Recommendations
- **Boost Subscriptions** → Promote exclusive benefits to increase subscriber base  
- **Customer Loyalty Programs** → Reward repeat buyers to strengthen loyalty  
- **Review Discount Policy** → Balance sales growth with margin control  
- **Product Positioning** → Highlight top-rated and best-selling products in campaigns  
- **Targeted Marketing** → Focus efforts on high-revenue age groups and express-shipping customers  

---

## 🚀 Tech Stack
- **Python** → pandas, matplotlib, seaborn  
- **PostgreSQL** → SQL queries & analysis  
- **Power BI** → dashboard visualization  

---

## 📂 Repository Structure
