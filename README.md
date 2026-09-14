# 📊 Customer Churn Analysis & Performance Dashboard

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-Data%20Analysis%20Expressions-blue?style=for-the-badge)
![Business Intelligence](https://img.shields.io/badge/Business%20Intelligence-Analytics-green?style=for-the-badge)

## 📌 Project Overview
Customer churn is one of the most critical metrics for subscription-based businesses. This Power BI project provides an end-to-end interactive dashboard designed to analyze customer churn patterns, identify high-risk customer segments, evaluate financial losses, and suggest actionable retention strategies.

---

## 📸 Dashboard Preview

### 1. Executive Summary & Churn Metrics
![Executive Summary](./screenshot_kpi.png)

### 2. Customer Demographics & Behavior Analysis
![Demographics & Services](./screenshot_demographics.png)

---

## 🔍 Key Insights & Business Findings

* **Contract Types:** Customers on **Month-to-month contracts** exhibit the highest churn rate compared to one-year or two-year contracts.
* **Payment Method Risk:** **Electronic Check** is associated with the highest churn rate (**45.29%**) and represents over **$84,000** in lost revenue.
* **Tenure Vulnerability:** Churn is heavily concentrated in the **first 1–5 months** of customer onboarding, indicating an early retention issue.
* **Service Impact:** Customers using **Fiber optic internet** and those **without Tech Support** show significantly higher churn tendencies.
* **Financial Impact:** Over **$139K** in cumulative revenue has been lost to churn across ~1,869 churned customers.

---

## 🛠️ Tech Stack & DAX Calculations

* **Tool:** Microsoft Power BI Desktop
* **Data Transformation:** Power Query (ETL, Data Cleaning & Type Casting)
* **Data Modeling:** Star Schema / Relational Model
* **Key DAX Metrics Used:**
  * **Churn Rate (%):** `DIVIDE([Churned Customers], [Total Customers], 0)`
  * **Revenue Lost to Churn:** `CALCULATE(SUM(Table[MonthlyCharges]), Table[Churn] = "Yes")`
  * **Month-over-Month (MoM) Growth:** Time Intelligence functions (`PARALLELPERIOD`, `DATEADD`)

---

## 💡 Strategic Recommendations

1. **Incentivize Long-term Contracts:** Offer discounts for moving from *Month-to-Month* to *Annual* contracts.
2. **Improve Onboarding Experience:** Implement proactive customer check-ins during the first 90 days (highest churn window).
3. **Promote Automated Payments:** Encourage Credit Card / Bank Transfer auto-pay options, as they show significantly lower churn rates than Electronic Checks.
4. **Bundle Tech Support:** Offer free introductory Tech Support packages with Fiber Optic subscriptions to resolve early technical friction.

---

## 🚀 How to View & Use

1. Clone or download this repository.
2. Open the `.pbix` file using [Power BI Desktop](https://powerbi.microsoft.com/desktop/).
3. Use the slicers (Gender, Senior Citizen, Partner, Dependents, Date) to filter and interact with the data dynamically.


## 👤 Author
* **GitHub:** [@marmatch](https://github.com/marmatch)
* **Role:** Data Analyst / Power BI Developer
