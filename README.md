# RetailMart Sales & Inventory Analytics

### End-to-End Data Analytics & Business Intelligence Project

**Transforming retail data into actionable insights for smarter business decisions.**

---

## Project Overview

RetailMart Sales & Inventory Analytics is an end-to-end data analytics capstone project designed to evaluate retail business performance using sales, product, customer, store, and inventory data.

The project analyzes synthetic retail data from **January 2024 to December 2025**, combining data cleaning, relational database development, SQL analysis, Python-based Exploratory Data Analysis (EDA), and interactive Power BI dashboards.

The goal is to identify sales trends, evaluate profitability, understand customer purchasing behavior, monitor inventory performance, and provide actionable business recommendations.

## Project Objectives

- Clean and preprocess raw retail datasets.
- Identify missing values, duplicates, and inconsistent records.
- Design a relational SQLite database.
- Perform SQL-based business analysis.
- Analyze revenue, gross profit, and year-over-year growth.
- Identify top-performing products, categories, stores, and regions.
- Understand customer purchasing patterns.
- Evaluate inventory efficiency and stock availability.
- Perform exploratory data analysis using Python.
- Develop interactive Power BI dashboards.
- Generate business insights and recommendations.

## Tools & Technologies

| Technology | Purpose |
|---|---|
| Microsoft Excel | Initial data inspection |
| Python | Data cleaning and exploratory analysis |
| Pandas & NumPy | Data manipulation and numerical operations |
| Matplotlib & Seaborn | Data visualization |
| SQLite | Relational database management |
| SQL | Data analysis and KPI calculations |
| Google Colab | Python development environment |
| Microsoft Power BI | Interactive dashboards |
| DAX | Business metrics and calculations |

## Dataset Overview

The project uses five synthetic retail datasets.

| Dataset | Cleaned Records |
|---|---:|
| Sales | 9,970 |
| Products | 60 |
| Customers | 3,000 |
| Stores | 6 |
| Inventory | 75,656 |

The datasets contain information about retail transactions, product categories, customer segments, store locations, and daily inventory activity.

## Project Workflow

### Phase 1 — Business Understanding

- Identified business problems and analytical requirements.
- Defined relevant key performance indicators.
- Established sales, customer, and inventory analysis objectives.

### Phase 2 — Data Cleaning & Preprocessing

Data cleaning was performed using Python and Pandas.

**Sales Cleaning:**
- Removed 12 duplicate transactions.
- Excluded 18 invalid quantity records.
- Identified 75 missing customer identifiers.
- Identified 45 missing payment methods.
- Preserved 47 invalid or unknown discounts as missing values.

**Inventory Cleaning:**
- Reconstructed 28 missing Stock_Received values.
- Removed one incomplete record.
- Excluded 23 inventory balance mismatches.
- Prepared 75,656 cleaned inventory observations.

### Phase 3 — SQLite Database Development

Created a relational database:

`RetailMart_Final_Analytics.db`

Developed analytical SQL views:

- `vw_sales_analysis` — 9,970 records.
- `vw_inventory_analysis` — 75,656 records.

Used SQL joins, filtering, aggregation, and business calculations to analyze retail performance.

### Phase 4 — Python Exploratory Data Analysis

Performed EDA using Python, Pandas, Matplotlib, and Seaborn.

Analysis included:

- Monthly and yearly revenue trends.
- Revenue by product category.
- Top-performing products.
- Store-wise and regional performance.
- Customer segment analysis.
- Inventory valuation and turnover.
- Stockout observations.

### Phase 5 — Power BI Dashboard Development

Developed four interactive dashboard pages:

1. Executive Overview
2. Sales Analysis
3. Customer Analysis
4. Inventory Analysis

### Phase 6 — Business Insights & Documentation

Prepared three project documents:

- Executive Summary
- Business Recommendations
- Final Project Documentation

---

## Key Performance Indicators

| KPI | Result |
|---|---:|
| Total Revenue | ₹24,560,144.11 |
| Gross Profit | ₹9,200,460.20 |
| Gross Profit Margin | 37.46% |
| Total Orders | 7,936 |
| Average Order Value | ₹3,094.78 |
| 2024 Revenue | ₹11,734,966.71 |
| 2025 Revenue | ₹12,825,177.39 |
| YoY Revenue Growth | 9.29% |
| Inventory Turnover (2024) | 1.38x |
| Inventory Turnover (2025) | 1.02x |

**Note:** Financial KPIs were calculated using transactions with valid discount information.

## Power BI Dashboards

### 1. Executive Overview

Provides a high-level summary of business performance.

**Visualizations:**
- Total Revenue
- Gross Profit
- Gross Profit Margin
- Total Orders
- Average Order Value
- Year-over-Year Revenue Growth
- Monthly Revenue Trend

**Screenshot:** `Executive_Overview.png`

### 2. Sales Analysis

Analyzes sales performance across products, stores, and regions.

**Visualizations:**
- Revenue by Product Category
- Top 10 Products by Revenue
- Store-Wise Revenue Performance
- Region-Wise Revenue Performance

**Screenshot:** `Sales_Analysis.png`

### 3. Customer Analysis

Explores purchasing behavior across customer segments.

**Visualizations:**
- Revenue by Customer Segment
- Average Order Value by Customer Segment
- Total Orders by Customer Segment

**Screenshot:** `Customer_Analysis.png`

### 4. Inventory Analysis

Examines stock movement, inventory valuation, and stockout observations.

**Visualizations:**
- Monthly Stock Movement — Received vs Sold
- Latest Inventory Value by Product Category
- Top 10 Products by Stockout Frequency

**Screenshot:** `Inventory_Analysis.png`

**Validation Note:** Monthly stock movement quantities displayed in Power BI require further investigation. These values should not be interpreted as confirmed inventory trends until the data and model relationships have been verified.

---

## Key Business Insights

### Revenue Performance

RetailMart generated approximately **₹24.56 million** in total revenue during 2024–2025.

Revenue increased by **9.29%** from 2024 to 2025.

### Profitability

The business generated approximately **₹9.20 million** in gross profit, with a gross profit margin of **37.46%**.

### Product Performance

- Electronics was the highest revenue-generating category.
- Monitor was the highest revenue-generating individual product.

### Store & Regional Performance

- RetailMart T Nagar generated the highest store-level revenue.
- The South region contributed the highest regional revenue.

### Customer Behavior

- Regular customers generated the highest revenue and order volume.
- New customers recorded the highest average order value.

### Inventory Efficiency

Estimated inventory turnover declined from **1.38x in 2024** to **1.02x in 2025**, suggesting an opportunity to improve stock efficiency.

## Business Recommendations

1. **Optimize Inventory Management:** Monitor slow-moving products, review reorder quantities, and improve stock planning.
2. **Improve Customer Retention:** Introduce loyalty programs and encourage repeat purchases.
3. **Strengthen Product Performance:** Prioritize consistently high-performing products and categories.
4. **Improve Store Performance:** Compare store-level results and identify operational improvement opportunities.
5. **Increase Average Order Value:** Introduce product bundles and cross-selling strategies.
6. **Monitor KPIs Regularly:** Use Power BI dashboards for periodic performance reviews.

---

## Repository Structure

```text
RetailMart-Sales-Inventory-Analytics/
│
├── README.md
│
├── 01_Data/
│   ├── Raw_Data/
│   └── Cleaned_Data/
│
├── 02_SQL/
│   ├── RetailMart_Final_Analytics.db
│
├── 03_PowerBI/
│   └── RetailMart_Sales_Inventory_Analytics.pbix
│
├── 04_Reports/
│   ├── RetailMart_Executive_Summary.pdf
│   ├── RetailMart_Business_Recommendations.pdf
│   └── RetailMart_Final_Project_Documentation.pdf
```

*The structure above represents the intended repository layout. Include only files that have been created and uploaded.*

## Project Limitations

- The project uses synthetic retail data rather than actual company records.
- Some sales records contain missing customer, payment, or discount information.
- Financial KPIs exclude transactions with invalid discount values.
- Inventory turnover values are estimates.
- Monthly inventory movement values in Power BI remain unverified.
- The analysis covers historical data rather than real-time operations.

## Future Enhancements

- Automated ETL pipelines.
- Sales and demand forecasting.
- Advanced customer segmentation.
- Customer lifetime value analysis.
- Automated Power BI refresh.
- Inventory replenishment optimization.
- Real-time retail analytics integration.

## Skills Demonstrated

**Data Analytics:** Data Cleaning, EDA, KPI Development, Business Insights

**SQL:** Database Design, Joins, Aggregations, Analytical Views

**Python:** Pandas, NumPy, Matplotlib, Seaborn

**Business Intelligence:** Power BI, DAX, Data Modeling, Dashboard Design

**Business Analysis:** Sales Performance, Profitability, Customer Analytics, Inventory Management

## Project Documentation

Detailed documentation is available in the `05_Reports` folder:

- RetailMart_Executive_Summary.pdf
- RetailMart_Business_Recommendations.pdf
- RetailMart_Final_Project_Documentation.pdf

---

## Conclusion

The RetailMart Sales & Inventory Analytics project demonstrates an end-to-end analytical workflow, from raw data preprocessing to database integration, Python analysis, and interactive Power BI reporting.

The project highlights practical applications of SQL, Python, and Power BI in evaluating retail business performance and generating actionable business insights.

**Project Status:** Analytical development and documentation completed; inventory movement validation pending.

---

**RetailMart Sales & Inventory Analytics | End-to-End Data Analytics Portfolio Project**
