# 📊 HR Analytics — Boosting Retention with Data Insights at Adecco India

> **A data-driven HR analytics case study examining employee attrition, satisfaction, and retention strategies across 1,470 employees using Excel and statistical analysis.**

---

## 📌 Table of Contents

- [Project Overview](#-project-overview)
- [Problem Statement](#-problem-statement)
- [Dataset](#-dataset)
- [Tools & Technologies](#-tools--technologies)
- [Project Requirements](#-project-requirements)
- [Analysis Performed](#-analysis-performed)
- [Key Insights](#-key-insights)
- [Dashboard Preview](#-dashboard-preview)
- [Challenges Faced](#-challenges-faced)
- [Recommendations](#-recommendations)
- [Stakeholders](#-stakeholders)
- [Project Structure](#-project-structure)
- [How to Use](#-how-to-use)

---

## 🏢 Project Overview

Adecco India, a mid-sized technology company with a workforce spanning Engineering, Marketing, Sales, and Customer Support, faced a growing employee attrition crisis — particularly among junior-level Sales employees. This project leverages HR data analytics to uncover the root causes of turnover and inform evidence-based retention strategies.

The analysis covers **1,470 employees** across **35 variables**, using Excel-based analytics, pivot tables, statistical functions, and interactive charts to generate actionable workforce intelligence.

---

## ❓ Problem Statement

**What is the problem?**  
Adecco India is experiencing unsustainably high employee turnover, especially in the Sales department among junior-level staff. This disrupts team dynamics, lowers morale, and reduces overall productivity.

**Why does it matter?**  
High attrition creates cascading costs — recruitment, onboarding, training, and lost institutional knowledge. Solving this improves workforce stability, performance consistency, and long-term business outcomes.

**Core Questions Addressed:**
- What is the overall and departmental attrition rate?
- Which demographic and job-related factors drive attrition the most?
- How do satisfaction scores, overtime, pay, and tenure correlate with turnover?
- What targeted interventions can reduce attrition risk?

---

## 📂 Dataset

| Property | Details |
|---|---|
| **Source** | [Kaggle — IBM HR Analytics Case Study](https://www.kaggle.com/datasets/bhanupratapbiswas/hr-analytics-case-study) |
| **Records** | 1,470 employees |
| **Variables** | 35 columns |
| **Format** | `.xlsx` (Excel) |

**Key Variables Used:**

| Column | Description |
|---|---|
| `Attrition` | Whether the employee left (Yes/No) |
| `Department` | Sales / R&D / Human Resources |
| `JobRole` | Role within the company |
| `MonthlyIncome` | Monthly salary |
| `OverTime` | Works overtime (Yes/No) |
| `JobSatisfaction` | Satisfaction score (1–4) |
| `WorkLifeBalance` | Work-life balance score (1–4) |
| `YearsAtCompany` | Tenure in years |
| `YearsSinceLastPromotion` | Promotion recency |
| `StockOptionLevel` | Stock compensation level (0–3) |
| `TrainingTimesLastYear` | Training sessions attended |
| `BusinessTravel` | Travel frequency |
| `MaritalStatus` | Single / Married / Divorced |
| `Age` | Employee age |
| `PerformanceRating` | Rating (1–4) |

---

## 🛠 Tools & Technologies

| Tool | Purpose |
|---|---|
| **Microsoft Excel** | Primary analysis, pivot tables, charts, formulas |
| **Excel PivotTables** | Department, role, and demographic breakdowns |
| **Excel Charts** | Bar, pie, scatter, histogram visualizations |
| **COUNTIF / AVERAGEIF** | Attrition rate and conditional aggregations |
| **CORREL Function** | Correlation analysis between attrition and key variables |
| **Conditional Formatting** | Heatmaps and data bars for quick pattern recognition |
| **Scatter Plots + Trendlines** | Relationship analysis (age vs. satisfaction, tenure vs. attrition) |
| **Data Validation & Filters** | Interactive dashboard filtering |

---

## ✅ Project Requirements

### Data Requirements
- HRIS data: employee demographics, employment history, compensation
- Performance management: ratings, goals, achievements
- Employee survey data: job satisfaction, engagement, work-life balance scores
- Exit interview data: stated departure reasons

### Metric Development
| Metric | Formula / Source |
|---|---|
| Attrition Rate | `(Employees Left / Total Employees) × 100` |
| Job Satisfaction Score | Average of `JobSatisfaction` column |
| Engagement Score | Derived from `JobInvolvement` ratings |
| Performance Rating | Average of `PerformanceRating` column |
| Average Tenure | Average of `YearsAtCompany` column |

---

## 🔍 Analysis Performed

### Basic-Level Analysis
1. **Overall Attrition Rate** — Calculated using `COUNTIF` and `COUNTA`
2. **Attrition by Department** — PivotTable grouping with calculated rate fields
3. **Average Age of Leavers** — `AVERAGEIF` on attrited employees
4. **Job Satisfaction by Role** — PivotTable with average satisfaction scores
5. **Gender-Based Attrition** — Cross-tabulation and optional t-test
6. **Average Income of Leavers** — `AVERAGEIF` on attrition = "Yes"
7. **Distance from Home Impact** — Scatter plot with trendline
8. **Performance Rating Distribution** — Histogram via PivotTable
9. **Overtime Headcount** — `COUNTIF` on OverTime = "Yes"
10. **Average Company Tenure** — `AVERAGE` on `YearsAtCompany`

### Medium-Level Analysis
1. **Top Attrition Drivers** — `CORREL` function across all numeric variables
2. **Job Involvement vs. Attrition** — PivotTable with attrition rate by involvement level
3. **Age vs. Job Satisfaction** — Scatter plot with linear trendline
4. **Marital Status Impact** — Cross-tabulation attrition by marital status
5. **Training Impact on Attrition** — PivotTable by `TrainingTimesLastYear`
6. **Work-Life Balance vs. Performance** — Scatter analysis
7. **Stock Options vs. Attrition** — PivotTable by `StockOptionLevel`
8. **Tenure vs. Job Satisfaction** — Scatter with trendline
9. **Business Travel vs. Satisfaction** — Average satisfaction by travel frequency
10. **Years Since Promotion vs. Performance** — Scatter analysis

---

## 💡 Key Insights

### 🚨 Attrition Findings
- **Overall attrition rate: 16.1%** — 237 out of 1,470 employees left
- **Sales has the highest departmental attrition at 20.6%**, followed by HR (19.0%) and R&D (13.8%)
- **Youngest employees (18–25) carry the highest attrition risk at 34.8%** — nearly 1 in 3 leave
- **Overtime is the strongest binary predictor**: employees on overtime leave at **30.5%** vs **10.4%** for those who don't

### 💰 Compensation & Benefits
- Leavers earn on average **less than the company median** — compensation is a clear retention lever
- Employees with **Stock Option Level 0** show the highest attrition; those with level 1–3 are significantly more loyal
- The **Sales department** has the highest average income ($6,959) yet the highest attrition, suggesting pay alone is insufficient

### 👔 Role-Level Findings
- **Laboratory Technicians (62 exits), Sales Executives (57), and Research Scientists (47)** account for over 70% of total attrition
- **Sales Representatives** have a disproportionately high exit count relative to their headcount

### 🧑‍🤝‍🧑 People & Engagement
- **Single employees leave at a much higher rate than married or divorced employees**
- **Lower job involvement** strongly correlates with higher attrition — disengaged employees are flight risks
- Employees who received **fewer training sessions** show elevated attrition — investment in development builds loyalty
- **Long commutes (DistanceFromHome)** correlate positively with attrition, particularly for junior employees

### ⏱️ Tenure & Promotion
- Attrition peaks in the **first 1–3 years** of tenure — onboarding and early engagement are critical
- Employees who haven't been promoted in **4+ years** show declining performance ratings and higher exit intent

---

## 📊 Dashboard Preview

The Excel dashboard (`Dashboard` sheet) includes:

- **5 KPI Cards** — Total Employees, Attrition Rate, Avg Income, Avg Age, Overtime Rate
- **8 Embedded Charts** — Department attrition, age group attrition, overtime impact, work-life balance, job role breakdown, gender split, income by dept, marital status
- **Summary Table** — Side-by-side department comparison across 7 metrics
- **Dark Professional Theme** — Navy palette optimized for executive presentations

---

## ⚠️ Challenges Faced

### 1. Data Imbalance in Attrition Labels
The dataset is heavily imbalanced — only ~16% of employees are labelled "Yes" for attrition. This required careful use of rate-based metrics rather than raw counts to avoid misleading conclusions.

### 2. Correlation vs. Causation
Many variables showed correlation with attrition but not causation. For example, distance from home correlates with exits, but it's unclear if commute directly causes attrition or is a proxy for seniority and job level. Framing insights carefully was essential.

### 3. Categorical Variable Handling in Excel
Variables like `MaritalStatus`, `BusinessTravel`, and `OverTime` required encoding or pivot-based transformation for correlation analysis — Excel's `CORREL` function only works on numeric data, so binary encoding was needed.

### 4. Multi-Factor Interactions
Single-variable analyses can be misleading. High attrition in Sales may be driven by a combination of overtime + lower stock options + lower job involvement rather than any single factor. Excel-only analysis limits multi-variate modeling.

### 5. Dashboard Design Constraints
Building an interactive, visually rich dashboard purely in Excel (without Power BI or Tableau) required careful use of hidden data ranges, merged cells, and chart anchoring to maintain layout stability.

---

## 🎯 Recommendations

### Immediate Actions (0–3 months)
- **Address overtime** — Audit workload distribution in Sales and R&D; consider hiring or redistributing tasks to reduce overtime dependency
- **Compensation review for junior Sales roles** — Benchmark against market rates; targeted pay adjustments for high-risk roles (Sales Reps, Lab Technicians)
- **Enhance onboarding** — Implement structured 90-day and 1-year programs specifically targeting the 18–35 age cohort, which shows the highest early-tenure exits

### Medium-Term Initiatives (3–12 months)
- **Expand stock option eligibility** — Extend level 1+ options to more employees, especially in high-attrition roles; data shows clear retention impact
- **Structured promotion pathways** — Establish transparent timelines for progression; flag employees past 3 years without a promotion for manager review
- **Training investment** — Increase training sessions for junior employees; those attending more sessions show significantly lower attrition
- **Remote/flexible work pilots** — Offer hybrid options for employees with long commutes (>15 km), reducing one of the key environmental attrition drivers

### Strategic Improvements (12+ months)
- **Predictive attrition model** — Move beyond Excel to Python/Power BI for a logistic regression or random forest model that can flag at-risk employees in real-time
- **Pulse survey program** — Implement quarterly short surveys (5–7 questions) to monitor job satisfaction and engagement trends continuously, not just annually
- **Manager effectiveness tracking** — Incorporate `YearsWithCurrManager` into performance reviews; poor manager relationships are an under-analysed exit driver
- **Exit interview standardisation** — Digitise and categorise exit interview data to feed back into the analytics pipeline and validate model predictions

---

## 👥 Stakeholders

| Type | Stakeholder |
|---|---|
| Internal | HR Department, Sales Department, R&D Department, Marketing, Customer Support, Senior Management |
| External | Recruitment Agencies, Training Providers |

---

## 📁 Project Structure

```
📦 Adecco-HR-Analytics/
├── 📊 Adecco_HR_Analytics.xlsx        # ⭐ MAIN PROJECT FILE — open this
│   ├── Dashboard                      # Interactive KPI dashboard with 8 charts
│   ├── Raw Data                       # Source dataset (1,470 rows × 35 cols)
│   ├── Basic Q&A                      # Answers to 10 basic analysis questions
│   ├── Medium Q&A                     # Answers to 10 medium-level questions
│   ├── Dept Analysis                  # Department-level attrition breakdown
│   ├── Gender Analysis                # Gender-based attrition analysis
│   ├── Overtime Analysis              # Overtime impact study
│   ├── Job Involvement                # Job involvement vs. attrition
│   ├── Training & Satisfaction        # Training impact analysis
│   ├── Age & Tenure Analysis          # Age group and tenure breakdowns
│   ├── Income Analysis                # Compensation analysis
│   ├── Marital Analysis               # Marital status impact
│   ├── Work-Life Balance              # WLB distribution and effects
│   ├── Environment Satisfaction       # Workplace environment scores
│   ├── Tenure Band Analysis           # Tenure cohort attrition rates
│   ├── Promotion Analysis             # Promotion recency impact
│   ├── Job Role Attrition             # Role-level attrition detail
│   └── Recommendations               # Strategic action items
└── 📘 README.md                       # This file
```

---

## 🚀 How to Use

1. **Clone or download** this repository
2. Open **`Adecco_HR_Analytics.xlsx`** in Microsoft Excel 2016 or later — this is the complete project
3. Start at the **Dashboard** sheet for the executive overview with all KPI cards and charts
4. Browse the individual analysis sheets (e.g., `Dept Analysis`, `Overtime Analysis`) to drill into specific topics
5. Refer to `Basic Q&A` and `Medium Q&A` for documented answers to all case study questions
6. The `Raw Data` sheet contains the full source dataset if you want to extend the analysis in Python or Power BI

> **Note:** Enable content if prompted. All charts and the dashboard are embedded natively in the Excel file — no add-ins or plugins required.

---

## 📚 References

- [IBM HR Analytics Dataset — Kaggle](https://www.kaggle.com/datasets/bhanupratapbiswas/hr-analytics-case-study)
- [SHRM Employee Turnover Benchmarks](https://www.shrm.org)
- [People Analytics: How Data Science is Transforming HR](https://hbr.org)

---

<div align="center">

**Built with Microsoft Excel · Designed for HR Analytics · Adecco India Case Study**

⭐ If this project helped you, consider giving it a star!

</div>
