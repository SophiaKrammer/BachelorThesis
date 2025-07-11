# Interpretable Machine Learning: Comparing SHAP and Counterfactual Explanations in Housing Price Prediction

This repository contains the code and results of a thesis project that compares two widely used post-hoc explainability methods—**SHAP (SHapley Additive Explanations)** and **Counterfactual Explanations**—with a focus on their interpretability for non-expert users in the domain of housing price prediction.

## Objective

The project investigates how SHAP and Counterfactual explanations differ in terms of:
- **Understandability**
- **Actionability**
- **Plausibility**
- **Cognitive effort**

All evaluations are based on example-based, visual analysis of selected prediction instances using an XGBoost regression model trained on real estate data.


## Dataset

The dataset used is the **[House Prices – Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data)** dataset from Kaggle.

It includes structured data such as:
- Living area
- Number of bathrooms
- Location variables
- Year built
- Air conditioning
- Road access

---

## Methodology

- **Model**: XGBoost Regressor
- **Explanations**:
  - SHAP values using `shap.TreeExplainer`
  - Counterfactuals using multi-objective optimization (NSGA-II) via the `DiCE` library

Both explanation methods are applied to the same prediction instances to ensure comparability.


