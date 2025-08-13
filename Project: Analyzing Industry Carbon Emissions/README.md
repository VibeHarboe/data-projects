# Carbon Emissions by Industry - SQL Insight on Product-Level PCFs

## 🧭 Context & Challenge:
This project explored publicly available carbon footprint data published on nature.com, covering Product Carbon Footprints (PCFs) from global companies across industries.
The challenge was to quantify and rank industry-level emissions, and to identify how many companies drive those emissions in the most recent year of available data.
The underlying data stemmed from lifecycle-based product emissions, stored in a normalized SQL table: product_emissions.

---

## 🧩 Objectives:
Aggregate CO₂-equivalent emissions (PCF) across industries
Count the number of reporting companies per industry
Rank industries by total footprint to highlight key polluters
Limit analysis to the most recent year available in the dataset

---

## 🛠️ Technical Approach (SQL):
Extracted the latest reporting year using a subquery
Filtered product_emissions by that year only
Used SUM() and COUNT(DISTINCT company) grouped by industry_group
Ordered results by total_industry_footprint descending
Rounded outputs for reporting clarity

---

<h3 style="font-family: Lato, sans-serif; font-size: 20px; font-weight: normal;">📊 Results & Business Value:</h3>

<table style="width:100%; border-collapse: collapse; font-family: Lato, sans-serif; font-size:16px; font-weight: normal;">
  <thead>
    <tr>
      <th style="padding: 12px; border-bottom: 2px solid #ccc; text-align: left;">Insight Area</th>
      <th style="padding: 12px; border-bottom: 2px solid #ccc; text-align: left;">Outcome</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="padding: 12px;">🏭 Highest-Emitting Sector</td>
      <td style="padding: 12px;">Materials industry with the largest total PCF share</td>
    </tr>
    <tr>
      <td style="padding: 12px;">🧮 Company Coverage</td>
      <td style="padding: 12px;">Tech-related sectors reported across 4 companies, Materials only 3</td>
    </tr>
    <tr>
      <td style="padding: 12px;">🌎 Global Emission Insight</td>
      <td style="padding: 12px;">6 industries included, enabling comparative policy focus</td>
    </tr>
    <tr>
      <td style="padding: 12px;">📈 Year-Specific Focus</td>
      <td style="padding: 12px;">Limited to most recent year ensures data relevance for ESG teams</td>
    </tr>
  </tbody>
</table>

---

## 🔍 Strategic Learnings:
This project demonstrated how structured SQL analysis can produce compliance-grade sustainability insights, based entirely on publicly available data.
By grouping and aggregating PCFs by industry, I highlighted where environmental impact is concentrated – and which sectors may require closer regulatory or investor scrutiny.
