# HR-Analytics-Dashboards
Interactive HR analytics dashboards providing insights into workforce metrics, employee performance, and training outcomes through data-driven visualization and KPI tracking


---

## Project Overview

This project analyzes a workforce dataset of **2,845 employees** across multiple departments, job titles, and business units. The goal is to uncover workforce trends, performance gaps, training effectiveness, and diversity insights to support strategic HR decision-making.

---

## File Structure

```
HR_ANALYTICS_DATASET.xlsx
│
├── Raw Data               # Original unprocessed dataset
├── Cleaned Data           # Processed dataset with derived columns
├── KPI Calculation        # Key Performance Indicator formulas
├── Sheet Design           # Layout and design planning
├── DSH_WF_OV              # Dashboard: Workforce Overview
├── DSH_EPE                # Dashboard: Employee Performance & Engagement
├── DSH_THR                # Dashboard: Training & HR Metrics
└── Insights & Recommendations  # Key findings and action items
```

---

## Data Cleaning & Feature Engineering

The raw dataset was cleaned and enriched with the following derived columns:

| Derived Column | Logic |
|---|---|
| `Training Efficiency` | `Efficient` if Training Outcome = "Completed", else `Inefficient` |
| `Performance Category` | `High Performer` → Exceeds \| `Meets Expectations` → Fully Meets \| `Low Performer` → Needs Improvement \| `PIP` |
| `Satisfaction Level` | `High` (≥4) \| `Medium` (≥3) \| `Low` (<3) |
| `Tenure` | Calculated in years from Start Date to today |
| `Engagement Level` | `High` (≥4) \| `Medium` (≥3) \| `Low` (<3) |
| `Age Group` | Under 30 \| 30–40 \| 41–50 \| 50+ |

---
## Dashboard Screenshots
# Workforce Overview Dashboard
This dashboard presents a structured view of overall workfoce composition, highlighting employee distribution across departments, job roles, and demographic segments. It supports workforce planning by identifying concentration risks, staffing imbalances, and organizational structure patterns.
![Worfoce Dashboard](images/workforce_dashboard.png)

## Key Performance Indicators (KPIs)

### Workforce Overview (DSH_WF_OV)
- Total Employees
- Average Employee Age
- Male vs. Female Headcount
- Average Tenure

### Employee Performance & Engagement (DSH_EPE)
- Average Engagement Score
- Average Satisfaction Score
- Average Work-Life Balance Score
- Average Employee Rating
- High Performer Count

### Training & HR Metrics (DSH_THR)
- Total Training Cost
- Total Training Programs
- Training Completion Rate
- Average Training Duration (Days)
- Successful Training Count

Training programs tracked:
- Customer Service
- Project Management
- Technical Skills
- Communication Skills
- Leadership Development

---

## Key Insights

1. **Production is the dominant department**, comprising 67.1% of total headcount — making it the most critical area to monitor.

2. **Gender imbalance at leadership level**: The workforce is 55.8% female, yet the Executive Office is nearly all-male (23 of 24), revealing a significant gender gap at the top.

3. **An aging workforce**: The average employee age is 49.4 years, with **48% of staff aged 50+**, posing a future risk of knowledge loss as this cohort approaches retirement.

4. **Heavy reliance on non-permanent staff**: Full-Time (35%), Contract (33.4%), and Part-Time (31.5%) — a near-even split that may impact long-term stability.

5. **Strong racial diversity**: Asian (21%), Black (20.4%), White (20.1%), Other (19.5%), and Hispanic (19%) are all near-equal across pay zones.

6. **Zone A outperforms**: Zone A employees have a higher average rating (3.01) compared to Zones B (2.95) and C (2.96), suggesting possible differences in management quality or compensation.

7. **Limited performance mobility**: 79.1% of employees "Fully Meet" expectations while only 12.2% exceed them, indicating constrained upward performance differentiation.

8. **Software Engineering anomaly**: Zero employees rated "Exceeds," zero on "Needs Improvement," and zero on PIP — yet the department has a **17.9% turnover rate**, suggesting incomplete performance data or high performers leaving before being rated.

---

## Recommendations

1. **Urgently investigate turnover in Production and Software Engineering** — conduct exit and stay interviews to identify root causes around workload, management quality, career growth, and compensation.

2. **Develop a female retention strategy** — review promotion equity, flexible work arrangements, and management practices; consider mentoring programmes for female employees.

3. **Address the leadership gender gap** — implement a structured leadership pipeline and succession planning programme to develop female talent into senior roles.

4. **Create a succession and knowledge-transfer plan** for the 48% of staff aged 50+, to prevent critical institutional knowledge loss as this generation retires.

5. **Launch a targeted engagement campaign** starting with Production and Admin Offices — introduce recognition programmes, clear career pathways, and manager effectiveness surveys. Study what the Executive Office does differently and replicate those conditions.

---

## Tools Used

- **Microsoft Excel** — Data cleaning, KPI formulas, dashboard design
- **Excel Functions** — `IF`, `COUNTIF`, `COUNTIFS`, `AVERAGE`, `COUNTA`, `SUM`, `YEARFRAC`, `ArrayFormula`

---

