# Timekeeping Compliance Risk Model

## Overview
This project builds a predictive model to identify employees at risk of future timekeeping compliance violations, with a focus on California meal break laws.

A synthetic dataset was created to simulate real-world workforce behavior, including clock-in/out patterns, break timing, overtime, and manager-level influence.

## Dataset
- 500 employees
- 40 managers
- 180 days of activity (~62,000 records)

Features include:
- scheduled vs actual work times
- break behavior
- overtime
- anomaly flags
- rolling behavioral trends

## Methodology
- Applied California meal break compliance logic
- Engineered rolling 7-day and 30-day behavioral features
- Built forward-looking risk label (next 30 days)
- Trained Logistic Regression and Random Forest models
- Tuned classification threshold for business usability

## Results
- ROC-AUC: ~0.81
- Precision: ~20%
- Recall: ~54%

## Key Insights
- Manager-level behavior was the strongest predictor (~40% feature importance)
- Repeated late clock-outs and anomaly patterns drive risk
- Static factors like department and location had minimal impact

## Business Impact
This model can be used to:
- proactively identify compliance risk
- prioritize HR interventions
- reduce legal exposure from labor violations

## Tech Stack
- Python
- Pandas
- Scikit-learn
- Jupyter Notebook

## Author
Sean Devlin
