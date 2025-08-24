🇨🇦 Canada COVID-19 Tracker (Tableau Dashboard)

This project provides an interactive Tableau dashboard to track COVID-19 cases and deaths across Canadian provinces from Jan 2020 to Jan 2023.
It allows users to analyze trends, compare regions, and monitor the pandemic’s impact in near real-time.

📊 Dashboard Preview

<img width="1577" height="790" alt="image" src="https://github.com/user-attachments/assets/7f690553-f540-4d66-95c3-61ab335883c8" />


📂 Dataset

Source: Publicly available COVID-19 dataset (Canada)

Duration: Jan 1, 2020 – Jan 21, 2023

Key Fields: Province, Cases, Deaths, Date, Repatriated Travellers

🔎 Key Insights

Ontario & Quebec reported the highest number of cases (over 1M each).

Alberta recorded 626K cases with significant spikes in late 2021.

Smaller provinces (Yukon, Nunavut, Northwest Territories) had relatively fewer cases but showed noticeable impact during peak waves.

Both cases and deaths followed similar upward trends, with clear surges during multiple waves.

The last 7 days in the dataset still showed 673 new cases and 12 deaths, highlighting ongoing impact.

⚡ Challenges & Solutions
Challenge	Resolution
Tableau showed both Canada overall total and Repatriated Travellers in bar graph	Used Sets to exclude Canada & Repatriated Travellers
Excel dataset stored values as running totals, leading to inflated sums in Tableau	Created a calculated field using MAX() to pick the correct daily total
Tableau aggregated running totals across all dates	Applied calculated field with MAX(Date) to ensure only the correct value was displayed

✅ By combining Sets and Calculated Fields, the dashboard now reflects accurate values and provides meaningful insights.

💡 Recommendations

Automate data refresh if linked to a live COVID-19 dataset for real-time updates.

Add filters for wave analysis (1st, 2nd, Omicron etc.).

Include per-capita metrics (cases/deaths per 100K population) for fairer provincial comparisons.

Enhance storytelling by adding annotations for major events (lockdowns, vaccine rollouts).

🚀 How to Use

Clone this repository

git clone https://github.com/your-username/covid19-canada-tracker.git


Open the Tableau workbook file (Canada_COVID19.twbx).

Interact with filters (province, cases vs deaths) to explore trends.
