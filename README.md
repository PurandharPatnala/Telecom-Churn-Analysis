# 📊 Telecom Churn Analysis Project

This project presents an end-to-end Telecom Customer Churn Analysis using **SQL** for data cleaning and transformation, and **Power BI** for insightful visualization. The objective is to uncover customer churn patterns and guide telecom companies in making data-driven decisions to improve customer retention.

---

## 📌 Project Objective

The main goal of this project is to analyze telecom customer behavior and identify churn drivers using cleaned and transformed data. This involves:

* Extracting and cleaning raw customer data using **SQL Server Management Studio (SSMS)**
* Transforming and enriching data for analytics
* Visualizing churn and revenue metrics using **Power BI**
* Identifying actionable insights to support business decision-making

---

## 🛠️ Tools & Technologies Used

| Tool                                | Purpose                                       |
| ----------------------------------- | --------------------------------------------- |
| SQL Server Management Studio (SSMS) | Data cleaning, transformation, and validation |
| Power BI Desktop                    | Interactive dashboards and visualizations     |
| GitHub                              | Version control and project publishing        |

---

## 🧠 Skills Applied

* SQL Data Cleaning & Transformation
* Advanced SQL Queries (`CASE`, `CTE`, `GROUP BY`)
* Data Type Conversion & Null Handling
* Power BI Report Design
* Data Modeling and Relationships
* Analytical Thinking & Data Storytelling

---

## 🗃️ Dataset Overview

The project uses a raw **Telecom Customer Churn dataset** which includes key fields such as `customerID`, `MonthlyCharges`, `TotalCharges`, `Contract`, `PaymentMethod`, and `Churn`.

### Key Tables Created:

1. **Telecom**

   * Raw data containing all customer-level information.

2. **Telecom\_Cleaned**

   * Cleaned and transformed dataset after:

     * Null value handling
     * Revenue segmentation
     * Tenure binning
     * Churn flag creation
     * Categorical column normalization

3. **Monthly Revenue Summary**

   * Aggregated monthly revenue by payment method.

4. **Average Spend Summary**

   * Average MonthlyCharges and TotalCharges across customers.

5. **Churn Rate Summary**

   * Churn rates segmented by contract type.

---

## ⚙️ Key SQL Operations

* ✅ Handled nulls and trimmed whitespace
* ✅ Converted `TotalCharges` from `VARCHAR` to `FLOAT`
* ✅ Removed duplicate `CustomerID`s
* ✅ Created binary `ChurnFlag` (Yes → 1, No → 0)
* ✅ Segmented revenue into High, Moderate, and Regular groups
* ✅ Grouped `Tenure` into bins
* ✅ Normalized categorical columns such as `Gender`
* ✅ Created a materialized view: `Telecom_Cleaned`
* ✅ Summarized churn and revenue metrics by various dimensions

---

## 📊 Power BI Dashboard Overview

### ✅ KPIs Displayed

* Total Customers
* Average Monthly Charges
* Churn Rate
* Total Revenue

### 📈 Visuals Included

| Visualization               | Insight                                     |
| --------------------------- | ------------------------------------------- |
| Churn Rate by Contract Type | Highest churn in month-to-month contracts   |
| Revenue by Payment Method   | Most revenue from Auto-pay methods          |
| Churn by Tenure Group       | Highest churn in first-year customers       |
| Revenue Segment Pie Chart   | High vs. Moderate revenue user distribution |
| Churn by Gender             | Minor variance in churn across genders      |
| Customer Count by Contract  | Majority of customers on monthly plans      |

### 🔀 Interactivity

* Slicers for Payment Method
* Dynamic filtering across visuals
* Customized tooltips and color themes

---

## 📌 Key Business Insights

* 📉 **33% churn rate**, mainly from customers with short tenure and monthly contracts
* 💳 **Electronic Check users** have the highest churn rate
* 💰 **High-revenue customers** are fewer but crucial for profit
* 🕒 **Tenure 0–1 year** customers are the most likely to churn
* 🎯 Improvement opportunities lie in offering better contract options and targeting long-term value clients

---

## ✅ Conclusion

This project demonstrates the complete data analytics lifecycle—from **data extraction and transformation in SQL** to **interactive visual storytelling in Power BI**. The insights can help telecom companies to:

* Enhance customer retention strategies
* Reduce churn through contract and service improvements
* Prioritize high-value customer segments for loyalty programs

---

## 📁 Repository Structure

```
├── SQL/
│   ├── Telecom_Cleaning.sql
│   ├── Monthly_Revenue_Summary.sql
│   ├── Average_Spend_Summary.sql
│   └── Churn_Rate_Summary.sql
│
├── PowerBI/
│   └── Telecom_Churn_Analysis.pbix
│
├── README.md
└── Screenshots/
    └── Dashboard_Overview.png
```

---

## 📎 License

This project is open-source and available under the [MIT License](LICENSE).

