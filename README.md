# Human Life Expectancy Prediction using Machine Learning Regression in R

## Overview
This machine learning project aims to predict human life expectancy by leveraging multiple linear regression models in R. The project involves preprocessing, exploratory data analysis (EDA), feature engineering, and model optimization to uncover the most impactful healthcare, lifestyle, and socioeconomic variables. 

The primary goal is to build a predictive model that accurately forecasts life expectancy and provides actionable insights for improving population health metrics.

## Project Objectives
1. **Explore Influencing Factors**: Analyze health, socioeconomic, and lifestyle features to evaluate their impact on life expectancy.
2. **Identify Key Predictors**: Utilize statistical and machine learning methods to rank the significance of variables such as GDP, adult mortality, and schooling.
3. **Optimize Regression Models**: Implement techniques like backward elimination and multicollinearity checks (Variance Inflation Factor - VIF) to improve model accuracy.
4. **Derive Policy Insights**: Based on the model, propose targeted interventions to improve life expectancy across different countries.

## Dataset
The dataset includes health, economic, and demographic variables from over 190 countries. It contains 2938 rows and 22 features, including adult mortality, BMI, schooling, and income composition.

- **Source**: 
  - [WHO Dataset Documentation](https://cdn.who.int/media/docs/default-source/gho-documents/global-health-estimates/ghe2019_life-table-methods.pdf)
  - [Kaggle Dataset](https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who)

## Technical Workflow
1. **Data Preprocessing**: Handled missing values via median imputation, and outlier detection with a focus on health-related variables like HIV/AIDS prevalence.
2. **Feature Engineering**: Created dummy variables for categorical features and normalized numeric data to facilitate regression.
3. **Exploratory Data Analysis (EDA)**: Visualized relationships between life expectancy and predictor variables using scatter plots, heatmaps, and correlation matrices.
4. **Model Building**: Implemented multiple linear regression models and optimized them using automated backward elimination to remove non-significant variables.
5. **Model Validation**: Used statistical tests such as F-test, Breusch-Pagan test, and Shapiro-Wilk test to evaluate model assumptions like normality and homoscedasticity.

## Model Performance
- **R² (Training)**: 0.9599
- **R² (Test)**: 0.9492
- **F-statistic**: 295.9
- **p-value**: 2.2e-16

### Statistical Tests Used:
- **F-test**: Tested the overall significance of the regression model.
- **Breusch-Pagan Test**: Assessed homoscedasticity (constant variance of errors).
- **Shapiro-Wilk Test**: Checked for normality in residuals.

## Key Findings
- **Top Predictors**: Schooling, adult mortality, income composition, BMI, and HIV/AIDS prevalence are identified as the most significant factors impacting life expectancy.
- **Recommendations**: Policy interventions should focus on improving educational access, reducing mortality rates, and addressing public health issues like HIV/AIDS to enhance life expectancy.

## R Packages Used
- `corrplot`
- `fastDummies`
- `caret`
- `data.table`
- `dplyr`
- `car`
- `lmtest`

## Conclusion
This machine learning regression project offers both predictive insights and data-driven recommendations for improving life expectancy. The final model showcases strong performance metrics and highlights critical variables for policymakers to focus on. Further research could expand on specific regional factors and cultural dynamics affecting life expectancy.

## How to Run
Clone the repository and execute the `Human Life Expectancy Prediction.R` script in R to reproduce the analysis.

```bash
# Clone the repository
git clone https://github.com/yourusername/Human-Life-Expectancy-Prediction-ML-Regression-R.git
