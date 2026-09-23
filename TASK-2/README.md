# E-Commerce Customer Segmentation, Revenue Analysis & Business Performance

## 📌 Project Overview

This project was completed as part of the **ShadowFox Data Analyst Internship – Intermediate Level Task 2**.

The objective of this project is to analyze an e-commerce transaction dataset and identify important patterns in **sales performance, customer behavior, product performance, geographic contribution, and customer value**.

The analysis includes data cleaning, exploratory data analysis, business KPI calculation, customer segmentation using RFM analysis, visualization, and business recommendations.

---

## 🎯 Objectives

The main objectives of this project are:

* Clean and prepare a real-world e-commerce dataset.
* Analyze overall business and revenue performance.
* Understand customer purchasing behavior.
* Identify repeat and one-time customers.
* Analyze product-level revenue and sales.
* Identify important geographic markets.
* Analyze monthly revenue trends.
* Segment customers using RFM analysis.
* Identify high-value and at-risk customer groups.
* Build an interactive Power BI dashboard.
* Generate actionable business recommendations.

---

## 📊 Dataset

**Dataset:** Online Retail II

**Source:** UCI Machine Learning Repository

The dataset contains transactional records from an online retail business.

### Main attributes

* Invoice
* StockCode
* Description
* Quantity
* InvoiceDate
* Price
* Customer ID
* Country

The dataset contains transactions from **2009 to 2011**.

---

## 🧹 Data Cleaning & Preparation

The original dataset contained duplicate records, missing values, cancelled transactions, invalid quantities, and invalid prices.

The following preprocessing steps were performed:

1. Combined the two yearly worksheets into one dataset.
2. Removed duplicate transactions.
3. Removed cancelled invoices.
4. Removed transactions with quantity less than or equal to zero.
5. Removed transactions with price less than or equal to zero.
6. Removed records without Customer ID.
7. Removed records without product descriptions.
8. Converted InvoiceDate into datetime format.
9. Created additional time-based features.
10. Calculated transaction-level revenue.

### Revenue Calculation

```text
Revenue = Quantity × Price
```

### Additional features created

* Revenue
* Year
* Month
* YearMonth
* DayOfWeek
* Customer Type

After cleaning, the dataset contained approximately **779,425 valid transaction records**.

---

## 📈 Key Business KPIs

| KPI                  |         Result |
| -------------------- | -------------: |
| Total Revenue        | £17,374,804.27 |
| Total Orders         |         36,969 |
| Total Customers      |          5,878 |
| Total Products       |          4,631 |
| Total Units Sold     |     10,513,952 |
| Average Order Value  |        £469.98 |
| Repeat Customer Rate |         72.39% |

---

## 👥 Customer Analysis

Customer purchasing behavior was analyzed by calculating the number of unique orders placed by each customer.

### Customer classification

Customers were divided into:

* One-Time Customers
* Repeat Customers

Results:

* One-Time Customers: **1,623**
* Repeat Customers: **4,255**
* Repeat Customer Rate: **72.39%**

Repeat customers generated the majority of total revenue.

The analysis also showed that the **top 10% of customers contributed approximately 63.90% of total revenue**, indicating a strong concentration of revenue among high-value customers.

---

## 🧠 RFM Customer Segmentation

RFM analysis was performed using:

* **Recency** – How recently a customer purchased.
* **Frequency** – How often a customer purchased.
* **Monetary** – How much revenue the customer generated.

Customers were segmented into five groups:

| Segment             | Customers | Approx. Revenue |
| ------------------- | --------: | --------------: |
| Champions           |     1,292 |         £12.53M |
| Loyal Customers     |     1,356 |          £3.08M |
| Potential Loyalists |     1,456 |          £1.24M |
| At Risk             |       967 |          £0.37M |
| Lost Customers      |       807 |          £0.16M |

The **Champions** segment generated approximately **72.09% of total revenue**, showing that a relatively small high-value customer group contributes a large portion of business revenue.

---

## 📅 Monthly Revenue Analysis

Monthly revenue was analyzed to identify changes and recurring patterns over time.

The analysis showed a recurring increase in revenue during approximately **September, October, and November** in both observed years.

The highest monthly revenue in the cleaned dataset was:

**November 2010 — £1,166,460.02**

The lowest monthly revenue was:

**February 2011 — £446,084.92**

This recurring pattern can help businesses plan inventory, marketing activity, and operational capacity around periods of higher observed demand.

---

## 🛍️ Product Analysis

Products were analyzed based on revenue and quantity sold.

### Top products by revenue

1. REGENCY CAKESTAND 3 TIER
2. WHITE HANGING HEART T-LIGHT HOLDER
3. PAPER CRAFT, LITTLE BIRDIE
4. JUMBO BAG RED RETROSPOT
5. ASSORTED COLOUR BIRD ORNAMENT
6. PARTY BUNTING
7. MEDIUM CERAMIC TOP STORAGE JAR
8. PAPER CHAIN KIT 50'S CHRISTMAS
9. CHILLI LIGHTS
10. JUMBO BAG STRAWBERRY

Non-product entries such as **POSTAGE** and **Manual** were excluded from product-level revenue analysis to keep the product ranking focused on actual merchandise.

---

## 🌍 Geographic Analysis

Revenue was analyzed by country.

The United Kingdom generated approximately:

**£14.39M**

This represented approximately:

**82.82% of total revenue**

This indicates that the observed revenue was highly concentrated in the UK market, while other countries contributed smaller portions of total revenue.

---

## 🔍 Key Insights

### 1. Strong repeat-customer base

Approximately **72.39% of customers were repeat customers**, indicating substantial repeat purchasing activity within the analyzed dataset.

### 2. Revenue concentration among high-value customers

The top 10% of customers generated approximately **63.90% of total revenue**.

This means customer value is not evenly distributed across the customer base.

### 3. Champions generate a large share of revenue

The Champions RFM segment generated approximately **72.09% of total revenue**.

### 4. Seasonal revenue pattern

Revenue increased noticeably during September–November in both observed years, with November 2010 recording the highest monthly revenue.

### 5. Strong UK market concentration

Approximately **82.82% of revenue came from the UK**, showing a high geographic concentration in the observed transactions.

### 6. At-Risk and Lost customers

There were **1,774 customers** classified as At Risk or Lost.

These groups generated a comparatively small share of total revenue, so customer reactivation efforts can be prioritized based on individual customer value rather than applying the same campaign to everyone.

---

## 💡 Business Recommendations

### 1. Strengthen high-value customer retention

Develop loyalty programs, personalized recommendations, and targeted offers for high-value customers, particularly Champions and Loyal Customers.

### 2. Convert Potential Loyalists

Potential Loyalists represent a sizeable customer group. Personalized product recommendations and incentives for another purchase could help encourage continued engagement.

### 3. Plan for high-revenue periods

The observed September–November revenue increase can be considered when planning:

* Inventory
* Marketing campaigns
* Staffing
* Promotional activity
* Supply chain capacity

### 4. Use targeted reactivation campaigns

Instead of targeting every At-Risk or Lost customer equally, prioritize customers based on previous monetary value, frequency, and recency.

### 5. Explore international markets

Since the UK contributes a large share of revenue, the business could evaluate opportunities in established non-UK markets while continuing to maintain its core UK customer base.

---

## 📊 Power BI Dashboard

An interactive Power BI dashboard was created to visualize the analysis.

### Dashboard components

* Total Revenue
* Total Orders
* Total Customers
* Total Products
* Average Order Value
* Repeat Customer Rate
* Monthly Revenue Trend
* Customer Segments
* Revenue by Customer Segment
* Top 10 Products by Revenue
* Top 10 Countries by Revenue
* Year filter
* Country filter

The dashboard allows users to interactively explore business performance across different years and countries.

---

## 🛠️ Tools & Technologies

### Programming & Analysis

* Python
* Pandas
* NumPy

### Visualization

* Matplotlib
* Seaborn
* Power BI

### Development Environment

* Visual Studio Code
* Jupyter Notebook

### Version Control

* Git
* GitHub

---

## 📁 Project Structure

```text
TASK-2/
│
├── dashboard/
│   ├── clean_ecommerce_data.csv
│   ├── rfm_customer_segments.csv
│   └── Ecommerce_Analysis_Dashboard.pbix
│
├── data/
│   └── online+retail+ii/
│       └── online_retail_II.xlsx
│
├── images/
│   ├── monthly_revenue_trend.png
│   ├── top_products_revenue.png
│   ├── top_countries_revenue.png
│   ├── customer_segments.png
│   ├── segment_revenue.png
│   ├── repeat_vs_onetime_customers.png
│   └── revenue_by_customer_type.png
│
├── notebooks/
│   └── ecommerce_analysis.ipynb
│
└── README.md
```

---

## 🔄 Analytical Workflow

```text
Raw Dataset
     ↓
Data Cleaning
     ↓
Data Preparation
     ↓
Feature Engineering
     ↓
Exploratory Data Analysis
     ↓
KPI Analysis
     ↓
Customer Analysis
     ↓
RFM Segmentation
     ↓
Product & Geographic Analysis
     ↓
Power BI Dashboard
     ↓
Business Insights
     ↓
Recommendations
```

---

## 📌 Conclusion

This project demonstrates how transactional e-commerce data can be transformed into meaningful business insights through data cleaning, exploratory analysis, customer segmentation, and interactive visualization.

The analysis identified important patterns in customer retention, revenue concentration, product performance, geographic contribution, and monthly sales behavior.

The Power BI dashboard provides an interactive way to explore these findings and supports data-driven business analysis.

---

## 👩‍💻 Author

**Aaslesha Madhuri Avvaru**

B.Tech – Computer Science Engineering (Data Science)

**ShadowFox Data Analyst Internship – Intermediate Level Task 2**
