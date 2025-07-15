# Calculus Grade Prediction

This project develops a predictive model for AP Calculus final grades using multiple linear regression and Bayesian modeling, based on academic and teacher-level variables.

## Objective

To predict student performance in Calculus using:
- Math PSAT score
- GPA
- Precalculus grade
- Precalculus teacher
- Course level (Honors/AP)

## Methods

- Standardized predictors and built a multiple linear regression model
- Checked assumptions with Breusch-Pagan and Shapiro-Wilk tests
- Developed a Bayesian linear model with priors for teacher and course effects
- Visualized parameter estimates and predicted letter grade probabilities

## 📈 Key Results

- **Best predictors**: Precalculus grade, GPA, PSAT score (in that order)
- **Bayesian β estimates** (credible intervals):
  - Precalc Grade: 0.425 (0.251, 0.594)
  - GPA: 0.331 (0.186, 0.476)
  - PSAT: 0.290 (0.177, 0.405)
- **Teacher effects**: Teacher 3 showed significantly lower outcomes
- **Course level**: Students in AP section performed slightly worse on average

## 🔍 Example Predictions

| Student | Predicted Grade | 95% CI       | P(A)   | P(B)   | P(C)   | P(F)   |
|---------|------------------|--------------|--------|--------|--------|--------|
| 1       | 95               | 87 – 103     | 0.886  | 0.113  | 0.000  | 0.000  |
| 2       | 87               | 78 – 95      | 0.207  | 0.732  | 0.061  | 0.000  |
| 3       | 82               | 74 – 91      | 0.035  | 0.668  | 0.295  | 0.002  |

## Skills Demonstrated

- R (tidyverse, MASS, Bayesian inference)
- Regression diagnostics & hypothesis testing
- Probabilistic prediction & uncertainty quantification
- Academic data analysis and communication

## Files

- `code/` – R Markdown script for analysis
- `report/` – Final PDF project write-up
- *Dataset is private*

---
