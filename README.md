# 📊 Sales & Operations Analytics Dashboard

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-2.0+-green.svg)
![Status](https://img.shields.io/badge/Status-Completed-success.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

## 📋 Project Overview

A comprehensive end-to-end data analysis project examining **192,921+ sales transactions** across multiple business dimensions. This project demonstrates proficiency in data wrangling, feature engineering, exploratory data analysis (EDA), and deriving actionable business insights to support strategic decision-making.

### 🎯 Business Objectives
- Identify top-performing customers, products, and regions
- Analyze supplier and employee performance metrics
- Evaluate order fulfillment efficiency and logistics
- Assess the impact of discount strategies on revenue and profitability
- Uncover correlations to inform pricing and sales strategies

---

## 🗂️ Dataset Description

| Dataset | Description | Records |
|---------|-------------|---------|
| `orders` | Transaction-level order data | 192,921 |
| `customers` | Customer demographics & industry | - |
| `employees` | Sales representative information | - |
| `products` | Product catalog with pricing | - |
| `suppliers` | Supplier details & ratings | - |

**Final Merged Dataset:** 192,921 entries × 54 columns

---

## 🛠️ Technical Implementation

### Tech Stack
Python | Pandas | NumPy | Matplotlib | Seaborn | Jupyter Notebook

text


### Data Cleaning & Preparation
- ✅ Converted date columns (`order_date`, `ship_date`, `delivery_date`) to datetime objects
- ✅ Handled null values in `ship_date` and `delivery_date`
- ✅ Imputed missing `city` values using mode ('Phoenix, AZ')
- ✅ Imputed missing `supplier_rating` values using mean imputation
- ✅ Successfully merged 5 datasets into a unified analytical view

### Feature Engineering
```python
# Derived Metrics
profit = total_amount - (quantity * unit_cost)
order_lead_time = delivery_date - order_date  # in days
shipping_time_days = ship_date - order_date   # in days
📈 Key Findings & Insights
💼 Customer Performance
Metric	Top Performer	Value
Revenue	Home Depot	$30.94M
Order Volume	Verizon Communications	1.69K units
🌍 Geographic Analysis
Top State: New York (highest revenue contribution)
Underperforming: Ohio & Michigan (require strategic intervention)
Market Split: Strong domestic performance; international markets need focus
📦 Product Performance
Category	Product	Performance
Highest Revenue	AutoCAD Business	$41M+
Highest Quantity	LG UltraWide 34WN80C	Top seller by units
🏭 Industry Analysis
Top Industries: Telecommunications & Healthcare
Growth Opportunity: Manufacturing sector
📊 Operational Metrics
Metric	Value
Cancellation Rate	3%
Return Rate	2%
Avg. Shipping Time	3.00 days
💡 Discount Impact Analysis
Slight discounts correlate with increased revenue
Zero-discount transactions showed significant losses
🔗 Correlation Insights
Variables	Correlation	Interpretation
Total Amount ↔ Discount	0.96	Strong positive relationship
Total Amount ↔ Profit	0.86	Higher transactions yield greater profits
📁 Project Structure
text

sales-operations-analytics/
│
├── 📂 data/
│   ├── raw/                    # Original datasets
│   └── processed/              # Cleaned & merged data
│
├── 📂 notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_feature_engineering.ipynb
│   └── 03_exploratory_analysis.ipynb
│
├── 📂 reports/
│   └── findings_summary.pdf
│
├── 📂 visualizations/
│   └── charts/
│
├── requirements.txt
├── README.md
└── LICENSE
🚀 Getting Started
Prerequisites
Bash

Python 3.9+
pip install -r requirements.txt
Installation
Bash

# Clone the repository
git clone https://github.com/yourusername/sales-operations-analytics.git

# Navigate to project directory
cd sales-operations-analytics

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter Notebook
jupyter notebook
Requirements.txt
text

pandas>=2.0.0
numpy>=1.24.0
matplotlib>=3.7.0
seaborn>=0.12.0
jupyter>=1.0.0
📊 Strategic Recommendations
Based on the analysis, the following actions are recommended:

Customer Strategy: Develop loyalty programs for top customers (Home Depot, Verizon)
Geographic Expansion: Invest in targeted marketing for Ohio & Michigan
Pricing Optimization: Implement strategic discount tiers based on correlation findings
International Growth: Develop market entry strategies for underperforming regions
Supplier Diversification: Increase procurement from Suppliers 6 & 8 to balance risk
🔮 Future Enhancements
 Implement predictive models for sales forecasting
 Build interactive dashboards using Power BI/Tableau
 Develop customer segmentation using clustering algorithms
 Create automated reporting pipeline
 Add time-series analysis for seasonal trends
👤 Author
Shivang Sagwaliya
