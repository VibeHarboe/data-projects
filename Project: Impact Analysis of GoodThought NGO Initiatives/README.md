# Impact & Funding Insight for NGO Projects - SQL Analysis (GoodThought)

## 🧭 Context & Challenge:
GoodThought is a global NGO working in education, healthcare, and sustainable development.
The challenge was to extract meaningful insights from a complex relational database covering assignments, funding, and donor behavior – to reveal which regions and initiatives had the most impact and financial support.

---

## 🧩 Objectives:
Identify the most impactful project per region (based on impact_score)
Rank projects with the highest donation volume by donor type
Combine funding and operational performance metrics
Deliver clean, prioritized insights for leadership and reporting

---

## 🛠️ Technical Approach (SQL):
Used WITH CTEs to isolate and rank performance data
Joined donations, donors, and assignments to connect funding with donor type
Applied ROW_NUMBER() partitioning to identify top impact per region
Aggregated donation volume by assignment_id and donor_type
Ordered final outputs by relevance: highest funding and impact

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
      <td style="padding: 12px;">💸 Top-Funded Projects</td>
      <td style="padding: 12px;">Assignment_3033 (Individual donor) with $3,840+ in the East region</td>
    </tr>
    <tr>
      <td style="padding: 12px;">🌍 Regional Impact</td>
      <td style="padding: 12px;">East & South had the highest <code>impact_score</code> projects</td>
    </tr>
    <tr>
      <td style="padding: 12px;">🧑‍🤝‍🧑 Donor Patterns</td>
      <td style="padding: 12px;">Organizations dominated funding in West & North regions</td>
    </tr>
    <tr>
      <td style="padding: 12px;">🔗 Data Integration</td>
      <td style="padding: 12px;">Connected donor type with project scope and regional outcomes</td>
    </tr>
    <tr>
      <td style="padding: 12px;">🧠 Strategic Targets</td>
      <td style="padding: 12px;">Enabled NGO to prioritize donor engagement by region and impact level</td>
    </tr>
  </tbody>
</table>

---

## 🔍 Strategic Learnings:
This project showed how relational SQL logic (joins, partitions, aggregations) can be used to inform funding strategy in a nonprofit setting.
By linking donation behavior with project results, I delivered actionable recommendations for targeting donors, allocating funds, and reporting regional success.
It’s a strong example of how clean, well-organized SQL logic can turn raw transactional data into decision-ready insight.
