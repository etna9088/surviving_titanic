# Who survived the Titanic?

# 🚢 Titanic Survival Prediction

A data analysis and predictive modeling project using the Titanic dataset to identify factors influencing passenger survival.

**Author:** Madina Kanafina  
**Date:** November 2024  
**Tools Used:** R, `ggplot2`, `dplyr`, `tidyr`, logistic regression, cross-validation

---

## 📂 Project Overview

This project explores the Titanic dataset to:
- Visualize survival patterns based on age, fare, sex, passenger class, and family aboard.
- Impute missing values.
- Build and compare logistic regression models to predict survival.
- Evaluate model accuracy using cross-validation.

---

## 📊 Key Analyses & Visualizations

- **Histograms** of Age and Fare by survival status.
- **Bar charts** for categorical variables: Pclass, Sex, SibSp, and Parch.
- **Interaction plots** between passenger class and gender.
- Analysis of variable importance based on survival rates.

---

## 🧠 Modeling Summary

Three logistic regression models were built:

### `Model 1`
- Predictor: Age (imputed)
- Accuracy: ~61.6%
- Weak performance due to using only one variable

### `Model 2`
- Predictors: Age, SibSp, Pclass, Sex
- Cross-validation error: 0.199
- Simple, yet effective

### `Model 3`
- Predictors: Interactions between Age, Pclass, Sex + SibSp
- Same error as Model 2 (0.199) but more complex

📌 *Conclusion:* Model 2 balances simplicity and performance and is preferred.

---

## 🧹 Data Cleaning & Preparation

- Converted numeric survival to logical (`TRUE/FALSE`)
- Used median imputation for missing age values
- Reshaped data for plotting using `pivot_longer()`

---

## 📁 Files

- `titanic_analysis.R`: Main R script for analysis, modeling, and visualization
- `train.csv`: Raw dataset (not included here, available via Kaggle)

---

## 🔍 Insights

- Women and children had higher survival rates.
- First-class passengers were far more likely to survive than third-class.
- Age, Fare, Sex, and Pclass are important survival predictors.

---

## 💡 Skills Demonstrated

- Data cleaning & wrangling (`dplyr`, `readr`)
- Data visualization (`ggplot2`)
- Logistic regression modeling
- Model evaluation with cross-validation (`cv.glm`)
- Interpreting predictors and model performance

---

## 📫 Contact

- [LinkedIn](https://www.linkedin.com/in/etna907/)
- Email: etna9088@gmail.com
