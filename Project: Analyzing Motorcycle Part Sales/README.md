# Net Revenue Analysis Across Warehouses - SQL Project (DataCamp)

## 🧭 Context & Challenge:
A motorcycle parts distributor operating across three warehouses needed insight into monthly net revenue per product line, segmented by warehouse and client type.
The company accepts multiple payment methods (each with different fees), and leadership requested a clearer view of wholesale revenue trends across locations and time periods.

---

## 🧩 Objectives:
Calculate net revenue by product line, month, and warehouse
Ensure only wholesale transactions are included
Account for payment method fees in revenue calculation
Present data in a clean, decision-ready format

---


## 🛠️ Technical Approach (SQL):
Used CASE logic to extract and format months from date
Filtered dataset to only include "Wholesale" clients
Grouped by product line, month, and warehouse
Calculated net revenue: SUM(total) - SUM(payment_fee)
Sorted results by product and revenue to highlight top categories

---

<h3 style="font-family: Lato, sans-serif; font-size: 20px; font-weight: normal;">📊 Results & Business Value:</h3>

<table style="width:100%; border-collapse: collapse; font-family: Lato, sans-serif; font-size:16px; font-weight: normal;">
  <thead>
    <tr>
      <th style="border-bottom: 2px solid #ccc; text-align: left; padding: 12px;">Insight Area</th>
      <th style="border-bottom: 2px solid #ccc; text-align: left; padding: 12px;">Outcome</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="padding: 12px;">🧾 Net Revenue Logic</td>
      <td style="padding: 12px;">Successfully accounted for payment method deductions</td>
    </tr>
    <tr>
      <td style="padding: 12px;">🏢 Warehouse Comparison</td>
      <td style="padding: 12px;">Clear monthly view of warehouse-specific revenue trends</td>
    </tr>
    <tr>
      <td style="padding: 12px;">🧩 Product Line Focus</td>
      <td style="padding: 12px;">Revealed high-margin product lines per warehouse</td>
    </tr>
    <tr>
      <td style="padding: 12px;">📅 Seasonal Trends</td>
      <td style="padding: 12px;">Identified variations in revenue over summer months (June–August)</td>
    </tr>
  </tbody>
</table>

---

##  🔍 Strategic Learnings:
This project reinforced how well-structured SQL queries can surface powerful, revenue-critical insights.
By combining conditional logic, grouping, and business-specific calculations, I delivered a lean, scalable model for monthly reporting that could support decisions in pricing, product strategy, and operational focus.
