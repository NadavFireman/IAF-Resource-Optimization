# Operational Resource Optimization System (IAF)

## Live Project Demo
Explore the interactive decision-support dashboard:
**[Interactive Dashboard (Base44)](https://skyward-ops-02d143a6.base44.app)**

*Demo data is fully synthesized and re-skinned as a fictional civilian company, per military information-security requirements.*

## Project Overview
Crew-scheduling optimization for Israeli Air Force (IAF) squadrons, developed under the constraints of the "Iron Swords" war. The project replaces fragile, manual Excel-based scheduling with a data-driven decision-support system: a full operational year — 52 weeks, ~2,800 missions, 39,000+ crew assignments, ~120 aircrew members — was analyzed to quantify workload imbalance and scheduling errors, and a linear-programming assignment model was formulated to power an interactive prototype for squadron commanders.

## Key Features & Methodology
- **Operations Research:** Binary linear-programming assignment model — 3 objective functions (workload balance, priority-weighted mission coverage, and their weighted combination) under 9 hard-constraint families (qualifications, medical fitness, availability, rest intervals, daily workload caps, instructor pairing). Full formulation in the report.
- **Exploratory Data Analysis (EDA):** Cleaned and profiled 52 weeks of operational logs — ~3× weekly load swings (444 → 1,202 assignments), 28.8% of yearly crew-week capacity left unassigned, and workload gaps of up to 14 vs. 2 tasks per crew member.
- **Statistical Analysis:** Pearson correlation (SciPy) linking weekly workload to ~1,000 recorded mis-assignments (52% qualification / 48% availability) — r≈0.72–0.76, confirming that overload directly degrades scheduling quality.
- **KPI Definition:** Quantified success targets — a 30% reduction in unassigned crew (baseline: 34.5/week) and in the max–min workload gap, ≤5 qualification errors/week (baseline: 9.8), and a ≥20% gain in user satisfaction.
- **Field Validation:** 8 in-depth interviews with squadron role-holders, operational debrief reviews, a benchmark against 4 academic studies, and 3 user-feedback sessions with unit commanders.

## Tools & Technologies
- **Programming:** Python
- **Libraries:** Pandas, NumPy, SciPy, Seaborn, Matplotlib
- **Application / UI:** Base44 (interactive decision-support dashboard prototype)
- **Methodologies:** Operations Research (Linear Programming), Statistical Analysis, Process Improvement

## Repository Content
- **`quantitative_data_analysis.ipynb`**: Data cleaning, weekly/monthly trend visualization, error profiling, and Pearson correlation analysis (heatmap, regression scatter plots).
- **`operational_metrics_data.xlsx`**: The anonymized dataset — 52 weekly records, 12 monthly aggregates, and a statistical-summary sheet.
- **`Project_Final_Report.pdf`**: The full academic report (Hebrew, with an English executive summary) — methodology, findings, the complete model formulation, system design, and commander feedback.

> **Note:** All data, names, units, and operational details have been synthesized and strictly anonymized to comply with military information-security regulations.

---
*Final Project (Grade: 92) — B.Sc. Industrial Engineering & Management, Shenkar College.*
