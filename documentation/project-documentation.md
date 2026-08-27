# Banking Loan Risk Analytics — Power BI

## 1. Project Overview

This project develops an interactive Power BI analytics solution for analysing applicant characteristics, loan application behaviour, credit exposure, and observed payment difficulty patterns.

The objective is to transform banking application data into a business-oriented dashboard that helps stakeholders understand portfolio composition, identify segments with higher observed risk, and translate those patterns into practical risk-management considerations.

> **Analytical scope:** This project is descriptive and diagnostic. It identifies patterns and associations in the analysed dataset; it is not a predictive credit-scoring or default-probability model.

## 2. Business Problem

Financial institutions need to monitor applicant and loan portfolios across multiple dimensions while quickly identifying segments that may require additional attention.

The analysis focuses on questions such as:

- How large is the applicant and credit portfolio?
- What proportion of applicants experience payment difficulty?
- How does payment difficulty vary by loan type?
- Which age and income segments show higher observed payment-difficulty rates?
- What applicant characteristics are associated with higher observed risk indicators?
- How do previous application outcomes and loan behaviour contribute to the overall risk picture?
- What practical actions could a business consider based on these observed patterns?

## 3. Project Objectives

1. Build an interactive banking risk analytics dashboard in Power BI.
2. Establish a clean and validated analytical data model.
3. Create reusable DAX measures for portfolio and risk KPIs.
4. Segment applicants across relevant demographic and financial characteristics.
5. Analyse application and loan behaviour.
6. Identify meaningful patterns in observed payment difficulty.
7. Translate analytical findings into business-oriented recommendations.

## 4. Dataset

The project uses a banking loan/application dataset containing applicant-level information and variables related to demographics, income, credit, applications, and payment-difficulty outcomes.

The analysis uses fields required to evaluate applicant characteristics, income and credit amounts, loan type, age groups, income groups, application history, risk indicators, and payment-difficulty outcome.

The final dashboard analyses **307,511 applicants** in the project dataset.

## 5. Data Preparation

Data preparation was performed in **Power Query** before modelling and reporting.

Key preparation activities included:

- Reviewing source tables and column structures
- Checking and standardising data types
- Cleaning and preparing analytical fields
- Creating categories required for segmentation
- Preparing fields for reliable relationships and filtering
- Validating transformed data before modelling

## 6. Data Model

A structured Power BI data model was created to support interactive analysis across applicants, applications, loan characteristics, and risk-related attributes.

The model was validated before dashboard development to ensure that relationships behaved as expected, filters propagated correctly, measures returned consistent results, and segmentation visuals reflected the intended population.

## 7. DAX & Analytical Measures

DAX was used to create reusable business measures rather than relying only on raw columns.

Core measures include:

- **Total Applicants**
- **Total Credit Amount**
- **Average Credit Amount**
- **Average Income**
- **Payment Difficulty Rate**
- Risk-segmentation measures
- Application and refusal-related measures
- Credit-to-income risk indicators
- External-risk segmentation measures

A key portfolio KPI is the observed payment-difficulty rate:

**Payment Difficulty Rate = Payment Difficulty Applicants / Total Applicants**

For the overall dataset, approximately **24,825 applicants** were classified with payment difficulty out of **307,511 applicants**, producing an observed rate of approximately **8.1%**.

## 8. Dashboard Structure

The final dashboard contains four pages designed as a progressive analytical story.

### Page 1 — Executive Overview

Provides the high-level portfolio view through total applicants, total credit exposure, average credit amount, average income, payment-difficulty rate, applicant outcome split, payment difficulty by loan type, age and income risk patterns, and key risk-segment indicators.

### Page 2 — Applicant & Risk Analysis

Moves from portfolio-level KPIs into applicant segmentation across dimensions such as age, income, education, occupation, and risk indicators. The objective is to identify where observed payment difficulty is concentrated rather than treating the entire applicant population as homogeneous.

### Page 3 — Loan & Application Behaviour

Examines application outcomes, previous application behaviour, loan characteristics, credit/application patterns, and approved versus refused behaviour. This adds behavioural context to the demographic and financial segmentation.

### Page 4 — Risk Insights & Recommendations

Converts the analysis into decision-support content through a payment-difficulty risk matrix, key analytical insights, business recommendations, and a methodology/interpretation note.

The page demonstrates the transition from **data → analysis → insight → action**.

## 9. Key Findings

### 9.1 Overall payment difficulty

Approximately **8.1%** of applicants in the analysed population are classified as experiencing payment difficulty. This provides the baseline against which different applicant and loan segments can be compared.

### 9.2 Loan type

The dashboard shows a higher observed payment-difficulty rate for **cash loans (8.3%)** than for **revolving loans (5.5%)**. This indicates that loan type is an important segmentation dimension for portfolio monitoring.

### 9.3 Applicant scale and credit exposure

The analysed population contains **307,511 applicants**, with approximately **184.21 billion** in total credit amount and an average credit amount of approximately **599.03K**. Average applicant income is approximately **168.80K**.

### 9.4 Age and income segmentation

The dashboard identifies differences in observed payment difficulty across age and income segments. These differences should be interpreted as descriptive associations within the analysed dataset rather than evidence that age or income directly causes payment difficulty.

### 9.5 Risk segmentation

The analysis also evaluates high credit-to-income and external-risk segments to identify applicant groups that may warrant closer monitoring.

## 10. Business Recommendations

### 1. Strengthen monitoring of higher-risk segments

Use observed payment-difficulty and risk-indicator patterns to prioritise monitoring and deeper review of segments with consistently elevated rates.

### 2. Incorporate loan-type differences into portfolio monitoring

Because payment-difficulty rates differ between cash and revolving loans, portfolio reporting and risk monitoring can include loan-type segmentation rather than relying only on an overall portfolio rate.

### 3. Use applicant segmentation for targeted risk management

Age, income, credit-to-income relationships, and external-risk indicators can be combined with broader underwriting information to support more targeted monitoring and assessment.

> These recommendations are analytical considerations, not lending-policy prescriptions. Actual credit decisions should incorporate a broader set of financial, behavioural, regulatory, and underwriting information.

## 11. Limitations

- The analysis is **descriptive**, not predictive.
- Observed relationships do not establish causation.
- The dashboard should not be interpreted as a production credit-scoring model.
- The dataset may not represent the full population or current lending conditions.
- No external macroeconomic, bureau, employment-history, or longitudinal repayment data were incorporated beyond the available dataset fields.
- Business decisions should not rely on any single dashboard metric in isolation.

These limitations distinguish analytical insight from unsupported predictive claims.

## 12. Tools & Technologies

- **Power BI Desktop**
- **Power Query**
- **DAX**
- Data modelling
- Interactive dashboard design
- KPI and risk segmentation

## 13. Analytical Workflow

```text
Raw Banking Data
       ↓
Data Inspection
       ↓
Power Query Transformation
       ↓
Data Model
       ↓
DAX Measures
       ↓
Risk & Applicant Segmentation
       ↓
Interactive Dashboard
       ↓
Analytical Insights
       ↓
Business Recommendations
```

## 14. Portfolio Value

This project demonstrates practical capabilities relevant to **Data Analyst, Business Analyst, BI Analyst, and entry-level Finance Analytics** roles.

It demonstrates the ability to:

- Work with a business-oriented dataset
- Prepare data for analysis
- Build a relational analytical model
- Write reusable DAX measures
- Design interactive Power BI dashboards
- Perform applicant and risk segmentation
- Interpret patterns rather than simply report numbers
- Translate analysis into business recommendations
- Communicate analytical limitations responsibly

## 15. Conclusion

The Banking Loan Risk Analytics project transforms applicant and loan data into a four-page Power BI decision-support dashboard.

The analysis establishes a portfolio-level baseline, explores applicant and application behaviour, identifies segments with different observed payment-difficulty rates, and translates those patterns into practical risk-management considerations.

The project demonstrates the complete analytics cycle:

> **Prepare → Model → Measure → Analyse → Visualise → Recommend**

## Project Status

**Dashboard:** Complete  
**Data preparation:** Complete  
**Data modelling:** Complete  
**DAX analysis:** Complete  
**Dashboard QA:** Complete  
**Documentation:** Complete
