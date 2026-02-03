# Graduate Admission Prediction – Machine Learning Regression

## Overview
This project applies machine learning regression techniques to predict a student’s probability of graduate admission based on academic and profile-related features. The study is based on a real-world case from Jamboree Education and focuses on building an interpretable and statistically valid regression model.

---

## Problem Statement
Given a student’s academic profile (test scores, GPA, research experience, etc.), predict the **Chance of Admit** and identify the most influential factors affecting graduate admissions.

---

## Dataset
**File:** `jamboree_admission.csv`

**Features:**
- GRE Score (out of 340)
- TOEFL Score (out of 120)
- University Rating (1–5)
- SOP Strength (1–5)
- LOR Strength (1–5)
- CGPA (out of 10)
- Research Experience (0 = No, 1 = Yes)

**Target Variable:**
- Chance of Admit (continuous value between 0 and 1)

A unique row identifier was removed to prevent data leakage.

---

## Machine Learning Approach
- Framed the problem as a supervised regression task
- Performed Exploratory Data Analysis to study distributions, outliers, and correlations
- Built a baseline Linear Regression model using Statsmodels
- Diagnosed feature multicollinearity using Variance Inflation Factor (VIF)
- Applied Ridge and Lasso regression to improve coefficient stability

---

## Model Diagnostics
The following Linear Regression assumptions were tested:
- Multicollinearity (VIF < 5)
- Mean of residuals approximately equal to zero
- Linearity between predictors and target
- Homoscedasticity of residuals
- Normality of residuals using histogram and Q–Q plot

---

## Model Evaluation
Model performance was evaluated on both train and test data using:
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score
- Adjusted R²

Train and test results were compared to ensure generalisation and avoid overfitting.

---

## Key Insights
- GRE score, TOEFL score, CGPA, and research experience are the strongest predictors
- Academic consistency is more impactful than a single high score
- Multicollinearity exists between test scores and CGPA and must be handled carefully
- Regularisation improves coefficient stability without significant performance loss

---

## Tools & Technologies
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Statsmodels
- Scikit-learn

---

## Business & ML Impact
- Built an interpretable admission probability prediction model
- Identified key features influencing admission outcomes
- Provided a robust baseline model for future advanced ML approaches

---

## Future Improvements
- Non-linear regression and tree-based models
- Feature interaction terms
- Cross-validation and hyperparameter tuning
- Inclusion of additional profile attributes such as work experience

---

## Author
**Prathmesh Raut**  
MSc Computer Science | Data Analyst | Data Science & Machine Learning Enthusiast
