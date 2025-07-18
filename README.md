# Happiness-Report-Analysis

## Happiness Prediction Model

The goal of this project is to identify the key factors that influence national happiness scores using data from the 2023 and 2015 World Happiness Reports. The project seeks to understand which socio-economic and political variables are most correlated with happiness, and how they can be used to build predictive models for to model future happiness.

Ultimately, this project aims to provide data-driven insights on what matters most to a nation's collective happiness, and how these findings can inform future policy and happiness globally.

---

## Data Cleaning & Preprocessing Techniques

- Removal of missing values using `na.omit()`
- Correlation matrix built with `cor()` to identify strong predictors
- Variable scaling and transformation for standardization
- Handling of multicollinearity using Variance Inflation Factor (VIF)
- Outlier detection and removal via Cook’s Distance and studentized residuals

---

## Visualization Tools

Implemented through `ggplot2`, `seaborn`, and `matplotlib` to explore data patterns:

- **Scatterplots**: to evaluate linear relationships  
- **Boxplots**: to identify spread and outliers  
- **Heatmaps**: to visualize correlation strength between variables  

---

## Predictive Models Used

- **Multiple Linear Regression (MLR)** to model happiness scores  
- **Interaction Terms** to capture complex variable relationships  
- **Model Selection** via:  
  - Backward Stepwise Selection (AIC)  
  - Mallows' Cp Criterion  

---

## Optimization & Evaluation

- **Outlier Analysis**: tested model robustness by removing influential points  
- **MPSE (Mean Prediction Squared Error)** used as primary evaluation metric  
- **Cross-Validation** across datasets from both 2023 and 2015 reports  
- **Interaction Models** outperformed others in predictive power for both years  

---

## Key Findings

Top Predictors of happiness:

- Social Support  
- GDP per Capita  
- Freedom to Make Life Choices  

Generosity and Perceptions of Corruption showed weaker or inconsistent correlations.

Models performed well within the 2023 dataset but struggled to generalize fully to 2015, revealing the complexity and contextual nature of happiness.

---

## Conclusion

This project shows how multiple regression models can be leveraged to understand and predict national happiness scores. Among all models tested, the Interaction Model produced the best fit and lowest prediction error, suggesting that happiness is influenced by how different factors work together—not just in isolation.

Happiness, much like health or education, appears to be multifactorial. Countries and policymakers should prioritize economic stability, strong social networks, and individual freedoms to meaningfully improve well-being.
