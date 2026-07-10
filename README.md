# Operational Resource Optimization System (IAF)

## Live Project Demo
**[Interactive Dashboard (Base44)](https://skyward-ops-02d143a6.base44.app)** — *runs on fully synthesized data, re-skinned as a fictional civilian company per military information-security requirements.*

## Project Overview
Crew-scheduling optimization for Israeli Air Force (IAF) squadrons, developed during the "Iron Swords" war. A full operational year — 52 weeks, 39,000+ crew assignments, ~120 aircrew members — was analyzed to replace manual Excel-based scheduling with a data-driven decision-support system, powered by a linear-programming assignment model and an interactive prototype for squadron commanders.

## Key Features & Methodology
- **Operations Research:** Binary linear-programming assignment model — 3 objective functions and 9 hard-constraint families (qualifications, medical fitness, availability, rest intervals, workload caps, instructor pairing); full formulation in the report.
- **Exploratory Data Analysis:** ~3× weekly load swings (444 → 1,202 assignments), 28.8% of crew-week capacity left unassigned, and workload gaps of up to 14 vs. 2 tasks per crew member.
- **Statistical Analysis:** Pearson correlation (SciPy) between weekly workload and ~1,000 recorded mis-assignments (52% qualification / 48% availability) — r≈0.72–0.76.
- **KPI Definition:** Quantified targets — a 30% cut in unassigned crew (baseline: 34.5/week), ≤5 qualification errors/week (baseline: 9.8), and a ≥20% gain in user satisfaction.
- **Field Validation:** 8 in-depth role-holder interviews, a benchmark against 4 academic studies, and 3 commander feedback sessions.

## Tools & Technologies
Python (Pandas, NumPy, SciPy, Seaborn, Matplotlib) · Base44 · Operations Research (Linear Programming), Statistical Analysis, Process Improvement

## Repository Content
- **`quantitative_data_analysis.ipynb`**: Data cleaning, trend visualization, error profiling, and correlation analysis (heatmap, regression scatters).
- **`operational_metrics_data.xlsx`**: Anonymized dataset — 52 weekly records, 12 monthly aggregates, and a statistical-summary sheet.
- **`Project_Final_Report.pdf`**: Full academic report (Hebrew + English executive summary) — methodology, findings, complete model formulation, and commander feedback.

---
*Final Project (Grade: 92) — B.Sc. Industrial Engineering & Management, Shenkar College.*
