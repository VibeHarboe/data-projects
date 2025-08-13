# Historical Business Longevity & Category Patterns - SQL Analysis Project

## 🧭 Context & Challenge:
This project explored a dataset compiled by BusinessFinancing.co.uk, covering the oldest existing businesses by country.
The main challenge was to identify patterns in business longevity across continents, categories, and countries – and to uncover what makes certain industries more resilient over time.
The data was stored in separate tables (businesses, countries, categories, new_businesses), requiring joins and conditional logic to create a unified, analytics-ready view.

---

## 🧩 Objectives:
Find the oldest operating business per continent
Identify which industries tend to survive the longest
Analyze global coverage gaps in available data
Combine datasets to compare historical vs. modern business data

---

## 🛠️ Technical Approach (SQL):
Used JOINs across 3 tables: businesses, countries, and categories
Built a WITH clause to combine businesses and new_businesses for global coverage analysis
Grouped data by continent and category to rank by founding year
Applied MIN() functions to extract earliest business by logic segment
Filtered for null values and used DISTINCT logic to isolate insights

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
      <td style="padding: 12px;">🌍 Oldest Global Industries</td>
      <td style="padding: 12px;">Agriculture, Distilling, Banking consistently rank oldest across continents</td>
    </tr>
    <tr>
      <td style="padding: 12px;">🗺️ Data Coverage</td>
      <td style="padding: 12px;">Identified countries per continent missing business history (e.g., Africa, Asia)</td>
    </tr>
    <tr>
      <td style="padding: 12px;">🧭 Resilient Categories</td>
      <td style="padding: 12px;">Hospitality, Manufacturing & Medical sectors found across centuries</td>
    </tr>
    <tr>
      <td style="padding: 12px;">📅 Temporal Analysis</td>
      <td style="padding: 12px;">Found active businesses dating back as early as 578 AD</td>
    </tr>
    <tr>
      <td style="padding: 12px;">🔗 Combined Sources</td>
      <td style="padding: 12px;">Created unified view of historical + modern business presence</td>
    </tr>
  </tbody>
</table>

---

## 🔍 Strategic Learnings:
This project highlighted how joined datasets and clean group-by logic in SQL can uncover deep patterns in real-world economic structures – across geography, industry, and time.
It also emphasized the importance of data completeness: only by merging and cleaning across sources could we identify blind spots in coverage and interpret results with confidence.
