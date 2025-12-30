# Dashboard – Sales, Cost, Profit Margin and KPI

## 1. Project Overview

This project presents an analytical dashboard developed in **Microsoft Power BI** with the objective of supporting business decision-making through the analysis of sales performance, logistics costs, profit, and profit margin over time.

The dashboard was developed as part of **LAB II – Chapter 3** of the *Microsoft Power BI for Business Intelligence and Data Science* program at **Data Science Academy (DSA)**.

The solution focuses on transforming raw transactional data into actionable insights using clear, business-oriented visualizations.

---

## 2. Business Questions

The dashboard was designed to answer the following business questions:

1. What is the total sales value by shipping mode?
2. Which markets have the highest average shipping cost?
3. Is the company meeting its monthly average sales value target of 350?
4. Which product category has the highest average profit?
5. How has the profit margin behaved over time?

---

## 3. Datasets

Four datasets in CSV format were provided for this analysis:

### 3.1 Customers

**Fields:**

* Customer ID (PK)
* Customer Name
* Segment
* City
* State
* Country
* Market
* Region

**Records:** 1,590
**Data Quality:** No null values, no blank fields, no duplicates

---

### 3.2 Products

**Fields:**

* Product ID (PK)
* Category
* Sub-Category
* Product Name

**Records:** 10,293
**Data Quality:** No null values, duplicate primary keys identified

---

### 3.3 Orders

**Fields:**

* Order ID (PK)
* Order Date
* Ship Date
* Ship Mode
* Order Priority

**Records:** 25,036
**Data Quality:** No null values, duplicate primary keys identified

---

### 3.4 Sales

**Fields:**

* Order ID (FK)
* Customer ID (FK)
* Product ID (FK)
* Sales Value
* Quantity Sold
* Shipping Cost

**Records:** 51,290
**Data Quality:** No null values, duplicate records identified

---

## 4. Data Preparation and Modeling

During the exploratory phase, duplicate primary keys were identified in the **Products** and **Orders** tables. Since duplicated primary keys compromise relational integrity in Power BI, these records were removed after validation.

Additionally, Power BI did not automatically recognize column headers, requiring manual application of the "Use First Row as Headers" option.

### 4.1 Calculated Measures (DAX)

Based on the business requirements, two additional measures were created:

```DAX
Profit = Sales[Sales Value] - Sales[Shipping Cost]
```

```DAX
Profit Margin (%) = ROUND(DIVIDE([Profit], Sales[Sales Value]) * 100, 2)
```

These measures enabled profit and margin analysis across categories, markets, and time.

---

## 5. Dashboard Visualizations

The dashboard includes the following visual components:

* **Waterfall Chart:** Total sales value by shipping mode
* **Treemap:** Average shipping cost by market
* **KPI Indicator:** Average sales value compared to target
* **Donut Chart:** Average profit by product category
* **Line Chart:** Profit margin trend over time

Each visualization was selected based on best practices in data visualization and is aligned with a specific business question.

<img width="1305" height="727" alt="Print LAB II - Versão 1 0 0" src="https://github.com/user-attachments/assets/ae09f4df-3378-4983-a1b4-08132df3009f" />

For a detailed explanation of the visualization rationale, see:

📄 **[Data Visualization Rationale](docs/data_visualization_rationale.md)**

---

## 6. Filters and Interactivity

The dashboard allows users to filter data by:

* Year
* Quarter
* Other temporal dimensions

These filters enable dynamic exploration of performance across different periods.

---

## 7. Tools and Technologies

* Microsoft Power BI
* DAX (Data Analysis Expressions)
* CSV datasets

---

## 8. Key Takeaways

* Shipping mode has a significant impact on total sales contribution
* Logistics costs vary considerably across markets
* The average sales value remains below the defined target
* Profitability differs substantially between product categories
* Profit margin shows fluctuations over time, requiring continuous monitoring

---

## 9. Author

**Leandro Álax**
Data Analytics | Business Intelligence | Power BI

---

## 10. Disclaimer

The datasets used in this project were provided exclusively for educational purposes by Data Science Academy and do not represent real company data.
---
For professional inquiries or collaboration opportunities,
leandroalax@hotmail.com
