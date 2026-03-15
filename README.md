# 📊 Customer Churn Analysis Dashboard

<div align="center">

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Business Intelligence](https://img.shields.io/badge/Business_Intelligence-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

**An interactive Power BI dashboard that analyzes customer churn patterns and delivers actionable retention insights.**

[📸 View Screenshot](#-dashboard-preview) · [📁 Dataset](#-dataset) · [🔍 Key Insights](#-key-insights) · [🐛 Report Issue](https://github.com/sohail189/customer-churn-analysis-dashboard/issues)

</div>

---

## 📝 Description

The **Customer Churn Analysis Dashboard** is a business intelligence solution built with **Power BI** that helps organizations understand *why* customers leave and *which* customer segments are most at risk.

By visualizing churn patterns across contract types, tenure, and monthly charges, this dashboard empowers business teams to make **data-driven retention decisions** — reducing revenue loss and improving customer lifetime value.

> 💡 **Business Problem:** Companies lose significant revenue when customers cancel subscriptions or stop purchasing. Identifying at-risk customers *before* they churn is critical to staying competitive.

---

## ✨ Features

- 📉 **Churn Rate Analysis** — Visual breakdown of overall churn rate with trend indicators
- 📋 **Contract Type Segmentation** — Churn comparison across Month-to-Month, One Year, and Two Year contracts
- 👥 **Customer Activity Summary** — KPI cards showing Total, Active, Churned, and Monthly Churn figures
- 📊 **Churn Distribution Chart** — Clear visual split between active and churned customers
- 💰 **Revenue Impact Analysis** — Impact of monthly and total charges on churn behavior
- 📆 **Tenure-Based Insights** — How customer age (tenure) affects their likelihood to churn
- 🎯 **Interactive Filters** — Slice data by contract type, tenure range, and charge brackets
- 💼 **Actionable Recommendations** — Built-in insights to guide retention strategy

---

## 📌 Key Metrics

| Metric | Value |
|---|---|
| 👥 Total Customers | **1,869** |
| 📉 Churn Rate | **26.5%** |
| 📆 Average Tenure | **17.98 months** |
| 💰 Avg Monthly Charges | **$64.76** |
| 💳 Avg Total Charges | **$2,283** |
| 🔴 Churned Customers | **~495** |
| 🟢 Active Customers | **~1,374** |

---

## 🔍 Key Insights

### 1️⃣ Contract Type is the Strongest Predictor
> Month-to-month customers churn at dramatically higher rates than one-year or two-year contract holders. Short-term flexibility comes at a retention cost.

### 2️⃣ Tenure Matters — Early Months are Critical
> Customers with **less than 12 months** of tenure show the highest churn rates. The first year of the customer relationship is the highest-risk period.

### 3️⃣ Higher Monthly Charges Drive Churn
> Customers paying above-average monthly charges — especially newer customers — are significantly more likely to churn. Pricing perception is a key driver.

### 4️⃣ Long-Term Contracts = Strong Retention
> Two-year contract holders have near-zero churn. Incentivizing customers to commit long-term is the most effective retention strategy.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| **Power BI Desktop** | Dashboard creation, DAX measures, interactive visuals |
| **Microsoft Excel** | Data source, initial data cleaning |
| **DAX (Data Analysis Expressions)** | Custom KPI calculations and measures |
| **Power Query** | Data transformation and shaping |

---

## 📁 Repository Contents

```
customer-churn-analysis-dashboard/
│
├── Customer_Churn_Dashboard.pbix   ← Power BI Dashboard file
├── customer_churn.csv              ← Customer dataset (CSV format)
├── Screenshot (102).png            ← Dashboard preview screenshot
└── README.md                       ← Project documentation
```

---

## 🗂️ Dataset

**File:** `customer_churn.csv`

The dataset contains **1,869 customer records** with the following key fields:

| Column | Description |
|---|---|
| `customerID` | Unique customer identifier |
| `tenure` | Number of months with the company |
| `Contract` | Contract type (Month-to-month / One year / Two year) |
| `MonthlyCharges` | Monthly billing amount |
| `TotalCharges` | Total amount billed to date |
| `Churn` | Whether the customer churned (Yes/No) |
| `PaymentMethod` | How the customer pays |
| `InternetService` | Type of internet service |
| `TechSupport` | Whether tech support is subscribed |
| `SeniorCitizen` | Whether customer is a senior citizen |

---

## 🖥️ Dashboard Preview

![Customer Churn Dashboard](Screenshot%20(102).png)

> *Interactive Power BI dashboard showing churn rate by contract type, customer distribution, and KPI summary cards.*

---

## 📦 How to Use

### Option 1 — View in Power BI Desktop

1. **Download** the repository:
   ```bash
   git clone https://github.com/sohail189/customer-churn-analysis-dashboard.git
   ```

2. **Open** `Customer_Churn_Dashboard.pbix` in **Power BI Desktop**
   - Download Power BI Desktop free: [powerbi.microsoft.com](https://powerbi.microsoft.com/desktop)

3. **Explore** the interactive dashboard — use slicers to filter by contract type, tenure, and charges

### Option 2 — Explore the Dataset

Open `customer_churn.csv` in **Excel** or **Python/pandas**:

```python
import pandas as pd

df = pd.read_csv('customer_churn.csv')
print(df.head())
print(f"Churn Rate: {df['Churn'].value_counts(normalize=True)['Yes']:.1%}")
print(f"Total Customers: {len(df)}")
print(df.groupby('Contract')['Churn'].value_counts(normalize=True))
```

---

## 💼 Business Impact

| Business Goal | How This Dashboard Helps |
|---|---|
| 🔴 Reduce Churn | Identify high-risk segments before they leave |
| 💰 Protect Revenue | Quantify revenue at risk from churning customers |
| 🎯 Target Retention | Focus campaigns on month-to-month customers |
| 📈 Improve Pricing | Understand how charges impact customer loyalty |
| 📋 Strategic Planning | Data-driven decisions for contract and pricing strategy |

---

## 📊 Dashboard Sections

### Section 1 — KPI Summary Cards
Four headline metrics at a glance: Total Customers, Active Customers, Churned Customers, Monthly Churn

### Section 2 — Churn by Contract Type
Bar chart comparing churn rates across Month-to-Month, One Year, and Two Year contracts

### Section 3 — Churn Distribution
Donut chart showing the ratio of active vs churned customers

### Section 4 — Tenure & Charges Analysis
Visuals showing how tenure and monthly charges correlate with churn risk

---

## 🤝 Contributing

Contributions and improvements are welcome!

1. **Fork** the repository
2. **Create** a new branch:
   ```bash
   git checkout -b feature/your-improvement
   ```
3. **Commit** your changes:
   ```bash
   git commit -m "Add: description of improvement"
   ```
4. **Push** and open a **Pull Request**

### 💡 Ideas for Contribution
- [ ] Add Python EDA notebook alongside the Power BI dashboard
- [ ] Build a machine learning churn prediction model
- [ ] Add Streamlit web app for real-time churn prediction
- [ ] Add more advanced DAX measures
- [ ] Extend dataset with more customer demographics

---

## 📄 License

This project is licensed under the **MIT License** — free to use, modify, and distribute with attribution.

---

## 📬 Contact

**Muhammad Sohail**
*Data Scientist | Machine Learning Enthusiast | BI Developer*

[![GitHub](https://img.shields.io/badge/GitHub-sohail189-181717?style=flat-square&logo=github)](https://github.com/sohail189)
[![Email](https://img.shields.io/badge/Email-sm7933294@gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:sm7933294@gmail.com)

🔗 **Project Link:** [https://github.com/sohail189/customer-churn-analysis-dashboard](https://github.com/sohail189/customer-churn-analysis-dashboard)

---

<div align="center">

Made with ❤️ using Power BI & Data Science

⭐ **If this project helped you, please give it a star!** ⭐

</div>
