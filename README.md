# Credit Risk Scorecard — Artha Finance (NBFC)
## Business Context
Artha Finance is a mid-size NBFC operating across Tier 2 cities in UP, Bihar, 
and MP. With a default rate of 8.3% against an industry average of 5.1%, the 
firm needed a data-driven approval framework to replace its current rule-based system.

## What This Project Does
Builds a machine learning scorecard that assigns each loan applicant to a risk 
band (Green/Amber/Red/Black) and recommends an approval policy for each segment 
— including interest rate tiers and conditions.

## Key Findings
- EXT_SOURCE_2 (external credit score) is the single strongest predictor of default
- 574 out of 593 AMBER-band applicants did not default — Artha Finance is leaving 
  ₹15.99 crore in interest income unrealised by over-penalising this segment
- Optimal approval threshold of 0.79 minimises total expected business cost

## Results
| Model | AUC Score |
|---|---|
| Logistic Regression | 0.7056 |
| Random Forest | 0.6875 |

## Dashboard
[View on Tableau Public](https://public.tableau.com/views/Artha-Finance-Credit-Risk-Scorecard/Dashboard1)

## Project Summary
[Download PDF Report](Riya_Singh_CreditRisk_ArthaNBFC.pdf)
## Tech Stack
Python, Pandas, Scikit-learn, Imbalanced-learn, Matplotlib, Seaborn, Tableau Public

## Project Structure
- 01_EDA.ipynb — Exploratory analysis with business insights
- 02_modelling.ipynb — Model building and threshold optimisation
- 03_business_analysis.ipynb — Risk scorecard and recommendations

## Data Source
Home Credit Default Risk — Kaggle
