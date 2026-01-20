# 📊 TechSolutionsCorp Sales & Operations Analytics

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
| `customers` | Customer demographics & industry | 8000 |
| `employees` | Sales representative information | 150 |
| `products` | Product catalog with pricing | 245 |
| `suppliers` | Supplier details & ratings | 33 |

**Final Merged Dataset:** 192,921 entries × 54 columns

---

## 🛠️ Technical Implementation

### Tech Stack
Python | Pandas | NumPy | Matplotlib | Seaborn | Jupyter Notebook

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
```
# 📈 Key Findings & Insights

## 💼 Customer Performance
| Metric         | Top Performer              | Value        |
|---------------|----------------------------|--------------|
| Revenue       | Home Depot                 | $30.94M      |
| Order Volume  | Verizon Communications     | 1.69K units  |

---

## 🌍 Geographic Analysis
- **Top State:** New York (highest revenue contribution)
- **Underperforming States:** Ohio & Michigan (require strategic intervention)
- **Market Split:**  
  - Strong domestic performance  
  - International markets require additional focus

---

## 📦 Product Performance
| Category          | Product                    | Performance              |
|------------------|----------------------------|--------------------------|
| Highest Revenue  | AutoCAD Business           | $41M+                    |
| Highest Quantity | LG UltraWide 34WN80C       | Top seller by units      |

---

## 🏭 Industry Analysis
- **Top Industries:** Telecommunications & Healthcare
- **Growth Opportunity:** Manufacturing sector

---

## 📊 Operational Metrics
| Metric              | Value       |
|--------------------|-------------|
| Cancellation Rate  | 3%          |
| Return Rate        | 2%          |
| Avg. Shipping Time | 3.00 days   |

---

## 💡 Discount Impact Analysis
- Slight discounts correlate with increased revenue
- Zero-discount transactions showed significant losses

---

## 🔗 Correlation Insights
| Variables                   | Correlation | Interpretation                          |
|----------------------------|-------------|------------------------------------------|
| Total Amount ↔ Discount    | 0.96        | Strong positive relationship             |
| Total Amount ↔ Profit      | 0.86        | Higher transaction values drive profit   |

---
👤 Author
Shivang Sagwaliya
