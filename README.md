# UK House Price Prediction

MSc Data Science dissertation project for regional UK house-price forecasting using machine learning, explainability and Power BI.

## Project Overview

This project investigates three-month-ahead regional UK house-price forecasting using official UK public datasets. The study combines economic indicators, regional house-price information and machine-learning methods within a chronological forecasting design.

The main regression task compares six approaches:

- Linear Regression
- Ridge Regression
- Lasso Regression
- Random Forest Regression
- XGBoost Regression
- Ensemble Regression

A supporting classification analysis was also conducted to examine whether future price movement could be classified as Increase or No Increase.

Explainability was addressed separately using Ridge Regression coefficients and Random Forest SHAP analysis.

## Data Sources

The project uses official public data from:

- HM Land Registry / UK House Price Index
- HM Land Registry Price Paid Data
- Bank of England Bank Rate
- ONS / Nomis labour-market statistics

The final integrated modelling dataset is included in the `data` folder.

## Repository Structure

- `UK_house_price.ipynb` – Main Google Colab / Python analytical notebook
- `data/` – Final integrated modelling dataset
- `outputs/` – Regression, classification, prediction, regional error and coefficient outputs
- `figures/` – Key analytical figures used to support the dissertation findings
- `dashboard/` – Final five-page Power BI dashboard
- `README.md` – Repository guidance and project overview

## Main Results

Ridge Regression achieved the lowest RMSE in the final regression comparison and was selected as the principal regression model.

The analysis also showed that recent house-price history was the dominant predictive signal. Regional prediction error varied across UK regions.

The supporting classification task produced substantially weaker predictive performance than the continuous regression task.

## Explainability

Two complementary explainability approaches were used:

- Ridge Regression coefficients for interpretation of the selected linear model
- Random Forest SHAP analysis for model-level feature importance and local contribution analysis

These methods are interpreted as predictive associations rather than causal effects.

## Power BI Dashboard

The final Power BI dashboard contains five pages:

1. Market Overview
2. Regression
3. Classification
4. Price Paid Data
5. Explainability

The dashboard file is available in the `dashboard` folder.

## Reproducibility

The main workflow is contained in `UK_house_price.ipynb`.

The notebook covers:

- data preparation
- dataset integration
- exploratory analysis
- feature engineering
- chronological train-test splitting
- regression modelling
- classification modelling
- model evaluation
- regional error analysis
- explainability
- output generation

The saved CSV outputs and analytical figures in this repository provide supporting evidence for the results presented in the dissertation.

## Software and Tools

- Python
- Google Colab
- pandas
- NumPy
- scikit-learn
- XGBoost
- SHAP
- Matplotlib
- Power BI

## Author

MSc Data Science Dissertation  
Leeds Beckett University
