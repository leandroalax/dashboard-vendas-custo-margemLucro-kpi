# Data Visualization Rationale – Sales, Cost, Profit Margin and KPI Dashboard

This document explains the rationale behind the selection and use of each visualization included in the **Dashboard – Sales, Cost, Profit Margin and KPI**, developed in Microsoft Power BI as part of LAB II – Chapter 3 at Data Science Academy.

## 1. Overview

The purpose of this dashboard is to support business analysis from a sales, logistics cost, profit, and profit margin perspective, enabling managers to assess operational efficiency and financial performance over time.

Each visual was selected based on the business question it needed to answer, prioritizing clarity, comparability, and decision-support value.

---

## 2. Visualization Rationale

### 2.1 Waterfall Chart – Total Sales by Shipping Mode

<img width="467" height="330" alt="Print LAB II - grafico cascata" src="https://github.com/user-attachments/assets/e2ee32b1-1ed0-483d-938e-2a849a5fb151" />

**Business question:** What is the total sales value by shipping mode?

**Rationale:**
The waterfall chart is well suited to show how individual components contribute to a cumulative total. In this context, it clearly illustrates how each shipping mode (Standard Class, Second Class, First Class, and Same Day) contributes to overall sales value.

**Business value:**
Enables quick identification of the most relevant shipping modes in terms of revenue contribution and supports logistics and commercial strategy decisions.

---

### 2.2 Treemap – Average Shipping Cost by Market

<img width="648" height="307" alt="Print LAB II - treemap" src="https://github.com/user-attachments/assets/7a2fd17a-3879-4cd1-a782-0d0f2d45beaf" />

**Business question:** Which markets have the highest average shipping cost?

**Rationale:**
Treemaps are effective for proportional and hierarchical comparisons. This visualization allows rapid comparison of average shipping costs across markets using area and color as visual cues.

**Business value:**
Supports the identification of markets with higher logistics cost pressure, informing pricing strategies, route optimization, or carrier renegotiations.

---

### 2.3 KPI Indicator – Average Sales Value vs Target

<img width="370" height="273" alt="Print LAB II - kpi indicator" src="https://github.com/user-attachments/assets/ca6b25d1-963e-4e83-84b6-c2b0c92bea69" />

**Business question:** Is the company meeting the monthly average sales value target of 350?

**Rationale:**
The KPI visual is appropriate for direct comparison between an observed value and a predefined target. It provides immediate feedback on whether performance is above or below the strategic objective.

**Business value:**
Facilitates executive-level communication and rapid assessment of performance against business goals.

---

### 2.4 Donut Chart – Average Profit by Product Category

<img width="361" height="307" alt="Print LAB II - grafico rosca" src="https://github.com/user-attachments/assets/1c987903-677c-42c0-beaf-66a8acacc799" />

**Business question:** Which product category has the highest average profit?

**Rationale:**
Donut charts are suitable for categorical comparisons with a limited number of categories. They enable proportional comparison without compromising readability.

**Business value:**
Highlights the most profitable product categories, supporting portfolio management, pricing decisions, and sales focus.

---

### 2.5 Line Chart – Profit Margin Trend Over Time

<img width="648" height="312" alt="Print LAB II - grafico linha" src="https://github.com/user-attachments/assets/0853f1c7-7e08-4ee1-875a-f21b78427151" />

**Business question:** How has profit margin behaved over time?

**Rationale:**
Line charts are the preferred option for time-series analysis, as they effectively reveal trends, volatility, and potential seasonal patterns.

**Business value:**
Allows continuous monitoring of margin stability and supports proactive corrective actions and strategic planning.

---

## 3. Final Considerations

The combination of multiple visualization types in this dashboard balances executive-level overview with analytical depth. Each visual serves a specific purpose, avoids redundancy, and maximizes the informational value delivered to end users.
