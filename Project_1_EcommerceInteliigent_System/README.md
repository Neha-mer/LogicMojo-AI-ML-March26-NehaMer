# Ecommerce Intelligence System

## Project Overview

The Ecommerce Intelligence System is a data analytics project designed to generate business insights from e-commerce transactional data. The project performs data cleaning, preprocessing, feature engineering, data integration, and exploratory data analysis (EDA) to understand customer behavior, sales performance, product demand, seller performance, and customer satisfaction.

The objective is to transform raw e-commerce datasets into actionable business intelligence that can support strategic decision-making.

---

## Business Goals

* Understand customer purchasing behavior.
* Identify high-value and repeat customers.
* Analyze revenue trends and sales patterns.
* Discover top-performing product categories.
* Evaluate seller performance.
* Measure customer satisfaction through reviews.
* Generate insights for improving operational efficiency and customer experience.

---

## Dataset Description

The project utilizes multiple datasets:

| Dataset              | Description                            |
| -------------------- | -------------------------------------- |
| Customers            | Customer information and demographics  |
| Orders               | Order lifecycle and purchase details   |
| Order Items          | Product-level order information        |
| Products             | Product catalog and specifications     |
| Payments             | Payment details for each order         |
| Reviews              | Customer review and rating information |
| Sellers              | Seller information                     |
| Location             | Geographic location data               |
| Category Translation | Product category translations          |

---

## Technology Stack

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## Project Workflow

### 1. Data Loading

All datasets are loaded into Pandas DataFrames for analysis.

### 2. Data Quality Assessment

Performed:

* Missing value analysis
* Duplicate record detection
* Data type validation
* Column standardization

### 3. Data Cleaning

#### Missing Values Handling

* Removed records with missing product dimensions.
* Filled missing product categories with `Unknown`.
* Processed missing values in product description attributes.

#### Duplicate Removal

Removed duplicate records across all datasets.

#### Data Type Conversion

Converted date-related fields into proper datetime format.

---

## Data Integration

Multiple datasets were merged into a unified master table using:

* Customer ID
* Order ID
* Product ID
* Seller ID

This consolidated dataset serves as the foundation for all business analyses.

---

## Feature Engineering

Several business metrics were derived:

### Order Metrics

* Total Order Value
* Delivery Time
* Delivery Time in Days
* Items Per Order

### Customer Metrics

* Customer Purchase Frequency
* Customer Lifetime Value (CLV)
* Average Order Value (AOV)
* Customer Segmentation

### Time-Based Metrics

* Order Month
* Order Day
* Order Hour

---

# Exploratory Data Analysis

## Customer Analysis

### New vs Repeat Customers

Analyzed customer retention by classifying customers into:

* New Customers
* Repeat Customers

### Customer Segmentation

Customers were segmented into:

* High-Value Customers
* Low-Value Customers

based on the 75th percentile of Customer Lifetime Value.

### Geographic Analysis

Identified states with the highest concentration of customers.

Insights generated:

* Customer distribution by state
* Regional demand patterns

---

## Revenue and Sales Analysis

### Monthly Revenue Trends

Analyzed:

* Revenue growth over time
* Monthly sales patterns

### Order Volume Trends

Evaluated:

* Number of orders per month
* Peak purchasing periods

### Purchase Behavior

Analyzed:

* Orders by weekday
* Orders by hour

to identify peak shopping times.

---

## Product Analysis

### Top Selling Categories

Identified categories with highest order volumes.

### Product Demand Distribution

Analyzed:

* Popular products
* Demand concentration

### Revenue Contribution

Evaluated category-wise revenue contribution.

---

## Seller Analysis

### Top Performing Sellers

Measured seller performance using:

* Total orders fulfilled
* Revenue generated

### Seller Revenue Analysis

Identified:

* Highest revenue-generating sellers
* Seller contribution to overall business

### Seller Distribution

Analyzed order distribution across sellers.

---

## Customer Review Analysis

### Review Score Distribution

Studied customer satisfaction through review ratings.

### Delivery Time vs Reviews

Analyzed relationship between:

* Delivery speed
* Customer ratings

### Low-Rated Sellers

Identified sellers associated with:

* Poor customer ratings
* Customer dissatisfaction

---

# Key Business Insights

The analysis helps answer:

* Who are the most valuable customers?
* Which product categories drive the most sales?
* Which sellers contribute the most revenue?
* When do customers shop the most?
* How does delivery performance impact customer satisfaction?
* Which regions generate the highest demand?

---

# Visualizations

The project includes multiple visualizations:

* Bar Charts
* Line Charts
* Histograms
* Count Plots
* Box Plots

Used to effectively communicate business insights.

---

# Project Structure

```text
Ecommerce-Intelligence-System/
│
├── Ecommerce_Intelligence_System.ipynb
├── datasets/
│   ├── customers.csv
│   ├── orders.csv
│   ├── order_items.csv
│   ├── products.csv
│   ├── payments.csv
│   ├── reviews.csv
│   ├── sellers.csv
│   ├── location.csv
│   └── category_translation.csv
│
├── README.md
└── requirements.txt
```

---

# Conclusion

This project demonstrates a complete data analytics workflow for an e-commerce business. By combining data cleaning, integration, feature engineering, and exploratory analysis, the system generates valuable insights into customer behavior, sales performance, product demand, seller effectiveness, and customer satisfaction.
