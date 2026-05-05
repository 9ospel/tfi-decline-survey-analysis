# TFI Fellowship Decline Analysis — Why High-Potential Candidates Say No
An end-to-end data analysis project examining why 163 high-potential candidates 
declined the Teach For India fellowship offer, built with Python, SQL, and 
Power BI to surface actionable insights for recruitment leadership.

---

## Key Findings

- **51% Conversion Leakage:** Half of the declined candidates had a joining likelihood score of 5/5 — TFI's primary challenge is keeping momentum after closing the offer.
- **Structural Financial Barriers:** Financial commitments account for ~30% of declines, indicating a segment of the talent pool that requires creative financial onboarding solutions rather than just better outreach.
- **Channel Optimization:** Engagement channels like Phone Calls and Group Interviews drive the highest emotional buy-in, whereas mass recruitment events show diminishing returns for high-intent candidates.

---

## Project Overview

This project analyzes why selected candidates declined the Teach For India Fellowship offer. The goal is to identify patterns in candidate drop-offs, uncover the major drivers behind decline decisions, and provide actionable recommendations to improve offer acceptance rates.

Using SQL, Python, and Power BI, this project transforms raw survey data into an interactive executive dashboard designed for recruitment and leadership teams.

---

## Business Problem

A significant number of high-potential candidates decline fellowship offers each year. Understanding the reasons behind these decisions is crucial for:

- Improving candidate conversion rates
- Enhancing recruiter effectiveness
- Optimizing regional recruitment strategies
- Refining candidate engagement throughout the selection process

---

## Strategic Recommendations

Based on the data deep-dive, the following interventions are proposed to reclaim high-intent candidates:

1. **Academic Deferral Policy:** Implement a 12-month deferral option for candidates accepted into top-tier Master's programs to prevent "Academic Churn".
2. **Financial Bridge Program:** Provide relocation and setup advances for low-income candidates to lower the barrier for the first two months of the fellowship.
3. **Stakeholder Townhalls:** Facilitate regional townhalls for parents/guardians to address concerns regarding fellowship prestige and safety.

---

## Dashboard Preview

### Page 1 — Executive Summary
![Executive Summary](https://github.com/9ospel/tfi-decline-survey-analysis/blob/main/screenshots/dashboard_overview.png?raw=true)

*Three KPI cards show 163 total declines, an average joining likelihood of 4.20/5, 
and 45 unique decline reasons. The likelihood distribution chart reveals that 83 
out of 163 candidates had a score of 5 — the headline finding of the project. 
Top decline reasons and alternative paths chosen are shown alongside.*

---

### Page 2 — Operational Drill-Down
![Operational Drill-Down](https://github.com/9ospel/tfi-decline-survey-analysis/blob/main/screenshots/decline_reasons.png?raw=true)

*Three slicers (Region, Recruiter, Decline Reason) allow recruitment managers to 
filter all visuals dynamically. India - North (56) and India - South (52) account 
for the majority of declines. The touchpoints chart shows Group Interview (152) 
and Phone Call (139) as the highest-converting channels, while Recruitment Events 
show near-zero impact.*

---

### Page 3 — Strategic Insights
![Strategic Insights](https://github.com/9ospel/tfi-decline-survey-analysis/blob/main/screenshots/strategic_insights.png?raw=true)

*The Strategic Deep Dive page surfaces two headline metrics: 51% High Intent 
Leakage (candidates at 5/5 likelihood who still declined) and 28% Academic Churn 
(higher education as the primary driver). Four proposed interventions are mapped 
across Education, Engagement, Family, and Financial categories with target impact.*

---

## Objectives

- Identify the most common reasons candidates decline the fellowship.
- Analyze alternative opportunities candidates choose instead.
- Measure regional variations in candidate declines.
- Evaluate recruiter-level decline patterns.
- Surface actionable insights for the recruitment team.

---

## Data

The dataset contains survey responses from 163 candidates who declined the 
TFI fellowship offer. Each response includes:

- Primary reason for declining
- Alternative path chosen (MBA, corporate job, etc.)
- Joining likelihood score at time of offer (1–5 scale)
- Region of the candidate
- Assigned TFI recruiter
- Engagement channel effectiveness ratings

> **Note:** All candidate data has been anonymised. Names and personal 
identifiers have been replaced with unique IDs before publication.

---

## Tools & Technologies

| Tool | Purpose |
|---|---|
| Python / Pandas | Data cleaning and transformation |
| SQL (SQLite) | Structured analysis and querying |
| Jupyter Notebook | Exploratory analysis and documentation |
| Microsoft Power BI | Interactive dashboard and visualisation |

---

## Methodology

1. **Data Cleaning (Python/Pandas):** Standardized categorical responses and implemented snake_case formatting for SQL-ready schema architecture. Missing values were handled and categories standardized.

2. **SQL Analysis:** Cleaned data was loaded into SQLite for structured querying. Key analyses included decline factor frequency, regional breakdowns, recruiter performance, and engagement channel effectiveness.

3. **Dashboard (Power BI):** Three-page interactive dashboard built for two audiences — an executive summary page for leadership and an operational drill-down page for recruitment managers.

---

## Recommendations

| Priority | Recommendation | Expected Impact |
|---|---|---|
| High | Introduce 48-hour post-offer follow-up protocol for likelihood-5 candidates | Reduce post-offer drop-off |
| High | Surface financial support mechanisms earlier in the process | Address ~30% of declines |
| Medium | Reallocate recruitment event budget to phone calls and group interviews | Improve touchpoint ROI |

---

## Repository Structure

```text
TFI-Candidate-Decline-Analysis/
│
├── data/
│   ├── raw/                # Original survey exports
│   └── processed/          # Cleaned CSVs for Power BI/SQL
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb   # Python cleaning pipeline
│   └── 02_sql_analysis.ipynb    # SQL querying & deep-dive
│
├── dashboard/
│   └── TFI_Candidate_Decline_Analysis.pbix
│
├── screenshots/
│   ├── dashboard_overview.png
│   └── decline_reasons.png
│
├── README.md
├── requirements.txt
└── .gitignore
--- 

## How to Run

1. Clone the repository
2. Install dependencies: `pip install -r requirements.txt`
3. Run the cleaning notebook: `notebooks/data_cleaning.ipynb`
4. Open SQL queries in any SQLite client: `sql/analysis_queries.sql`
5. Open the dashboard: `dashboard/TFI_Candidate_Decline_Analysis.pbix` 
   (requires Power BI Desktop — free download from Microsoft)