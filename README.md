# Banking Loan Risk Analytics | Power BI

> **Portfolio Project 3 — Banking & Credit Risk Analytics**
>
> **Status: Dashboard Complete | Documentation & Portfolio Packaging**

An end-to-end Power BI analytics project built around the **Home Credit Default Risk** dataset. The project analyses applicant characteristics, loan exposure, payment difficulty, previous application behaviour, and risk segments to turn portfolio data into actionable business insights.

The goal is not to build a predictive credit-scoring model, but to use **descriptive and diagnostic analytics** to identify observed patterns associated with payment difficulty and support better risk-monitoring decisions.

---

## 📌 Project Overview

Financial institutions need to understand not only how much credit is being issued, but also **which applicant segments show higher observed payment difficulty and what historical behaviours may provide additional context**.

This project uses Power BI to transform raw banking application data into an interactive four-page analytical dashboard covering:

- Portfolio-level KPIs
- Applicant and risk segmentation
- Loan and application behaviour
- Payment difficulty patterns
- Historical application outcomes
- Business insights and recommendations

The project follows a complete BI workflow from data preparation and modelling through DAX, visualization, analysis, and decision-oriented reporting.

---

## 🎯 Business Objective

The primary objective is to analyse applicant and loan characteristics to answer practical business questions such as:

- What is the overall size and credit exposure of the analysed portfolio?
- What proportion of applicants experience payment difficulty?
- Which loan types show higher observed payment difficulty?
- How does payment difficulty vary across age and income segments?
- Which applicant characteristics are associated with higher observed risk?
- What can previous application behaviour tell us about the applicant profile?
- Which segments should receive closer risk monitoring?

---

## 📊 Dataset

**Dataset:** Home Credit Default Risk

The main application dataset contains **307,511 applicant records** used for the portfolio analysis.

The project also incorporates historical application information to provide additional behavioural context.

### Key analytical fields include

- Applicant income
- Credit amount
- Loan type
- Age
- Income group
- Education
- Occupation
- Previous application outcomes
- Payment difficulty indicator
- External risk indicators

> **Analytical note:** Payment difficulty is treated as an observed outcome in the dataset. The analysis identifies associations and patterns; it does **not** establish causation or predict future default probability.

---

## 🔄 Data Preparation

Data preparation was performed in **Power Query** before building the analytical model.

Key activities included:

- Loading and profiling source data
- Reviewing column types and data quality
- Standardizing data types
- Handling fields required for analysis
- Creating analytical groupings such as age and income bands
- Preparing fields required for risk segmentation
- Validating the transformed data before modelling

---

## 🧩 Data Model

A structured Power BI data model was created to support interactive analysis across applicant, loan, risk, and historical application dimensions.

The model was validated before dashboard development to ensure that filters and measures behaved consistently across the report.

---

## 🧮 DAX & Analytical Measures

DAX was used to create reusable business measures rather than relying only on raw columns.

Key analytical measures include:

- **Total Applicants**
- **Total Credit Amount**
- **Average Credit Amount**
- **Average Income**
- **Payment Difficulty Applicants**
- **Payment Difficulty Rate**
- **High Credit-Income Risk Applicants**
- **High External Risk Applicants**
- Previous application and refusal metrics
- Risk and segmentation measures used throughout the dashboard

The measures were designed to remain responsive to report filters and segmentation selections.

---

# 📈 Dashboard

The final report contains **four interactive pages**, each serving a different analytical purpose.

### 1. Executive Overview

Provides a high-level view of the portfolio through:

- Applicant volume
- Total credit exposure
- Average credit amount
- Average income
- Payment difficulty rate
- Applicant outcome split
- Loan-type risk comparison
- Age and income risk patterns
- Risk segment indicators

**Purpose:** Give decision-makers a quick understanding of portfolio scale and observed risk patterns.

### 2. Applicant & Risk Analysis

Explores how observed payment difficulty varies across applicant characteristics and risk segments.

Key dimensions include:

- Age
- Income
- Education
- Occupation
- Risk indicators
- Applicant segmentation

**Purpose:** Identify applicant groups requiring closer risk monitoring.

### 3. Loan & Application Behaviour

Analyses loan characteristics and historical application behaviour to provide additional context around applicant risk.

The page examines areas such as:

- Loan type
- Previous application outcomes
- Approved vs. refused applications
- Credit requested vs. approved
- Historical application behaviour

**Purpose:** Understand how loan and historical application patterns relate to observed payment difficulty.

### 4. Risk Insights & Recommendations

Converts the analytical findings into a concise decision-support view containing:

- Payment difficulty matrix by age and income
- Key risk insights
- Business recommendations
- Analytical limitations / methodology note

**Purpose:** Translate descriptive analysis into practical business actions.

---

## 🔍 Key Findings

The dashboard highlights several important observed patterns:

### 1. Younger applicants show higher payment difficulty

Payment difficulty is highest among the youngest applicant groups. The observed rate is approximately **12.3% for applicants under 25**, compared with approximately **5.2% among applicants aged 55+**.

### 2. Cash loans show higher payment difficulty

The observed payment difficulty rate is higher for **cash loans (~8.3%)** than for **revolving loans (~5.5%)**.

### 3. Overall payment difficulty is a minority outcome

Approximately **8.1%** of the analysed applicants are classified as experiencing payment difficulty, while the large majority fall into the non-difficulty outcome group.

### 4. Applicant segmentation provides additional risk context

Combining age, income, loan characteristics, and external risk indicators provides a more useful view of portfolio risk than relying on a single KPI.

### 5. Historical application behaviour adds context

Previous application outcomes can provide additional descriptive context when assessing applicant profiles, particularly when considered alongside current application characteristics.

> These findings describe patterns observed in the analysed dataset. They should not be interpreted as causal relationships or as evidence of future default probability.

---

## 💡 Business Recommendations

Based on the observed patterns, the dashboard recommends:

### 1. Segment-based risk monitoring

Monitor higher-risk applicant segments more closely, particularly combinations of age, income, and other observed risk indicators rather than relying on a single demographic attribute.

### 2. Credit exposure review

Give additional attention to segments and loan categories showing higher observed payment difficulty when reviewing credit exposure and portfolio risk.

### 3. Use historical behaviour as a supporting signal

Incorporate previous application outcomes as supporting context alongside current applicant and loan characteristics rather than treating historical outcomes as a standalone decision rule.

---

## 🛠️ Tools & Technologies

- **Power BI Desktop**
- **Power Query**
- **DAX**
- **Data Modelling**
- **Interactive Data Visualization**
- **Business & Risk Analytics**

---

## 📂 Repository Structure

```text
banking-risk-analytics-power-bi/
│
├── README.md
│
├── documentation/
│   └── project-documentation.md
│
├── screenshots/
├── executive-overview.png
├── applicant-risk-analysis.png
├── loan-application-behaviour.png
└── risk-insights-recommendations.png
│   
└── assets/
```

The `screenshots/im.pdf` file contains the dashboard visual reference used during final review.

---

## ⚠️ Limitations

- This project is **descriptive/diagnostic**, not a machine-learning default prediction model.
- Observed associations do not establish causation.
- The analysis is based on the available dataset and its historical characteristics.
- Real-world lending decisions would require additional information, validation, regulatory considerations, and production-grade credit-risk modelling.

---

## 📌 Project Takeaway

This project demonstrates how Power BI can be used to move from **raw banking data → data preparation → modelling → DAX → interactive analysis → risk segmentation → business recommendations**.

Rather than focusing only on dashboard aesthetics, the project emphasizes **business questions, analytical reasoning, risk interpretation, and decision-oriented communication**.

---

## 👤 Author

**Aryan Singhai**  
Mechanical Engineer transitioning into **Data Analytics & Business Analytics**

**Focus:** Data Analytics | Business Analytics | Power BI | SQL | Excel

---

⭐ If you find this project useful, feel free to explore the repository and dashboard documentation.
