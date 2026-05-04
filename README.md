# TFI Fellowship Decline Analysis — Why High-Potential Candidates Say No
An end-to-end data analysis project examining why 163 high-potential candidates 
declined the Teach For India fellowship offer — built with Python, SQL, and 
Power BI to surface actionable insights for recruitment leadership.

---

## Key Findings

- **51% Conversion Leakage:** Half of the declined candidates had a joining likelihood score of 5/5 — TFI's primary challenge is closing the offer, not building awareness[cite: 1].
- **Structural Financial Barriers:** Financial commitments account for ~30% of declines, indicating a segment of the talent pool that requires creative financial onboarding solutions rather than just better outreach[cite: 1].
- **High-Impact Touchpoints:** Phone calls and group interviews drive the highest emotional buy-in (reaching ~150 candidates), while mass recruitment events show diminishing returns for top-tier talent[cite: 1].

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

1. **Data Cleaning (Python/Pandas):** Raw survey data contained multi-select 
   responses separated by semicolons. These were exploded into individual rows 
   to enable accurate frequency analysis. Missing values were handled and 
   categories standardised.

2. **SQL Analysis:** Cleaned data was loaded into SQLite for structured querying. 
   Key analyses included decline factor frequency, regional breakdowns, recruiter 
   performance, and engagement channel effectiveness.

3. **Dashboard (Power BI):** Three-page interactive dashboard built for two 
   audiences — an executive summary page for leadership and an operational 
   drill-down page for recruitment managers.

  

## Repository Structure

```text
TFI-Candidate-Decline-Analysis/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── ├── notebooks/
│       ├── 01_data_cleaning.ipynb
│       └── 02_sql_analysis.ipynb
│
├── sql/
│   └── analysis_queries.sql
│
├── dashboard/
│   └── TFI_Candidate_Decline_Analysis.pbix
│
├── screenshots/
│   ├── dashboard_overview.png
│   ├── decline_reasons.png
│   └── recruiter_analysis.png
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