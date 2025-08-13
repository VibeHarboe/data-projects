# Product Insight & Churn Risk Analysis Using SQL

## 🧭 Context & Challenge:
As part of my practical SQL certification exam, I worked with raw product data from FoodYum – a fictional grocery retailer navigating inflation-driven consumer behavior.
The dataset had significant data quality issues and gaps that prevented business users from analyzing product availability, pricing strategies, and customer accessibility.

---

## 🧩 Objectives:
Clean and structure the dataset for reliable analysis
Identify missing/incomplete product records and fix them using business rules
Enable KPI tracking of product distribution, category performance, and price ranges
Support decision-making around pricing, customer segmentation, and inventory optimization

---

## 🛠️ Technical Approach:
SQL-based Data Cleaning: Detected and handled nulls, removed outliers, fixed datatype mismatches
Business Logic Imputation: Median-based imputation for numeric fields, categorical fallback for types
Data Enrichment: Added derived columns for analysis (e.g., price/weight ratio, category coverage)
Exploratory SQL Queries: Filtered, grouped and ranked product performance across dimensions
Churn Risk Flagging: Used filters to highlight product types at risk of customer drop-off

---

<h3 style="font-family: Lato, sans-serif; font-size: 20px; font-weight: normal;">📊 Results & Business Impact:</h3>

<table style="width:100%; border-collapse: collapse; font-family: Lato, sans-serif; font-size:16px; font-weight: normal;">
  <thead>
    <tr>
      <th style="border-bottom: 2px solid #ccc; text-align: left; padding: 12px;">Insight Area</th>
      <th style="border-bottom: 2px solid #ccc; text-align: left; padding: 12px;">Outcome</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="padding: 12px;">📦 Data Quality</td>
      <td style="padding: 12px;">+100% completeness across all key fields</td>
    </tr>
    <tr>
      <td style="padding: 12px;">📊 Product Mix</td>
      <td style="padding: 12px;">Identified key categories with pricing gaps (e.g., Premium Dairy)</td>
    </tr>
    <tr>
      <td style="padding: 12px;">💡 SKU Focus</td>
      <td style="padding: 12px;">Highlighted high-volume products lacking clear categorization</td>
    </tr>
    <tr>
      <td style="padding: 12px;">⚠️ Risk Signals</td>
      <td style="padding: 12px;">Flagged 170 products with missing <code>year_added</code> (i.e. no pricing traceability)</td>
    </tr>
  </tbody>
</table>


---

## 🔍 Strategic Learnings:
This project demonstrated the importance of structured SQL logic in preparing datasets for business use.
It also confirmed that data cleaning is not just technical – it’s a strategic step that determines what the business can see, understand and act on.
Even without visual tools, SQL alone delivered powerful insight into churn risk, price positioning and SKU health.
