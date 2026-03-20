# 📊 Customer Shopping Behavior Analysis

## 🔍 Overview

This project analyzes customer shopping behavior using transactional data from **3,900 purchases** across multiple product categories. The objective is to uncover insights into customer segments, spending patterns, product preferences, and subscription behavior to support data-driven business decisions. 

---

## 📁 Dataset

* **Rows:** 3,900
* **Columns:** 18
* **Key Features:**

  * Customer demographics (Age, Gender, Location, Subscription Status)
  * Purchase details (Item, Category, Amount, Season, Size, Color)
  * Behavioral data (Discount usage, Purchase frequency, Review rating, Shipping type)
* **Data Quality:**

  * 37 missing values in *Review Rating* handled using median imputation per category 

---

## 🛠️ Tools & Technologies

* **Python** (Pandas, NumPy) → Data cleaning & preprocessing
* **SQL (MySQL / PostgreSQL)** → Business analysis & querying
* **Power BI** → Dashboard and data visualization

---

## ⚙️ Project Workflow

### 1. Data Preparation (Python)

* Loaded dataset using Pandas
* Performed initial exploration using `.info()` and `.describe()`
* Handled missing values using category-based median
* Standardized column names (snake_case)
* Feature engineering:

  * Created **age_group**
  * Derived **purchase_frequency_days**
* Removed redundant columns (e.g., promo_code_used)

---

### 2. SQL Analysis (Business Insights)

Executed structured SQL queries to answer key business questions:

* Revenue comparison by **gender**
* Identified **high-spending customers using discounts**
* Top 5 products by **average rating**
* Comparison of **shipping types (Standard vs Express)**
* Subscribers vs Non-subscribers:

  * Total customers
  * Average spend
  * Revenue contribution
* Identified **discount-dependent products**
* Customer segmentation:

  * New, Returning, Loyal
* Top 3 products per category
* Repeat buyers vs subscription behavior
* Revenue contribution by **age group**

---

## 📊 Dashboard (Power BI)

An interactive dashboard was built to visualize insights:

### Features:

* KPI Cards:

  * Total Customers
  * Average Purchase Amount
  * Average Rating
* Visualizations:

  * Revenue & Sales by Category
  * Customer Distribution (Subscription Status)
  * Revenue & Sales by Age Group
* Filters:

  * Subscription Status
  * Gender
  * Category
  * Shipping Type

---

## 📈 Key Insights

* Majority of customers are **non-subscribers**, contributing higher total revenue
* **Clothing** category generates the highest revenue and sales
* **Young Adults** contribute the most to overall revenue
* Discount usage significantly influences purchasing behavior
* Loyal customers form the largest segment

---

## 💡 Business Recommendations

* **Boost Subscriptions:** Offer exclusive benefits to increase subscriber base
* **Customer Loyalty Programs:** Convert repeat buyers into loyal customers
* **Optimize Discount Strategy:** Balance promotions with profitability
* **Product Positioning:** Promote top-rated and best-selling products
* **Targeted Marketing:** Focus on high-revenue age groups and express-shipping users 

---

## 🚀 Conclusion

This project demonstrates an end-to-end data analytics pipeline:

* Data cleaning → SQL-based business analysis → Interactive dashboard
* Highlights the ability to extract actionable insights and present them effectively for decision-making

---

## 📌 Future Improvements

* Implement predictive models (customer churn, segmentation)
* Automate data pipeline
* Deploy dashboard for real-time analytics

---
