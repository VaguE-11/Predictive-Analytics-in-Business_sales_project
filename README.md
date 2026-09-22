# MIS444 - BigMart Sales Prediction

## Project overview
This course project applies predictive analytics to a retail sales problem. The objective is to predict `Item_Outlet_Sales`, a continuous sales outcome, using product and outlet characteristics from the BigMart Sales Prediction dataset.

## Workflow
1. Data loading and quality checks
2. Missing-value treatment
3. Duplicate checks
4. Categorical normalization and feature engineering
5. IQR-based outlier analysis
6. Exploratory data analysis (EDA)
7. Feature selection / permutation importance
8. Multiple regression models
9. Random Forest hyperparameter optimization with RandomizedSearchCV and 5-fold cross-validation
10. Test-set evaluation using MAE, MAPE, MSE, RMSE, and R2
11. Business interpretation and recommendations

## Models
- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- HistGradientBoosting Regressor
- Optimized Random Forest

## Final model
The executed analysis selected **Optimized Random Forest** using the lowest test RMSE criterion.

## Key results
- Optimized Random Forest MAE: **717.03**
- Optimized Random Forest MAPE: **55.51%**
- Optimized Random Forest MSE: **1,050,935**
- Optimized Random Forest RMSE: **1,025.15**
- Optimized Random Forest R2: **0.613**

Compared with the unoptimized Random Forest, optimization reduced RMSE by approximately **3.96%** and increased R2 by approximately **0.033**.

## Key findings
- `Item_MRP` had the highest permutation importance in the executed analysis.
- `Outlet_Type` was the second strongest permutation-importance feature.
- Supermarket Type3 had the highest average sales among outlet types in the EDA (3,694.04).
- Starchy Foods had the highest average sales among item types in the EDA (2,374.33).

## Repository contents
- `notebooks/` - final Colab/Jupyter notebook should be placed here
- `figures/` - EDA and model-diagnostic charts
- `results/` - CSV outputs from the executed analysis
- `report/` - final course report

## AI usage disclosure
AI tools were used as learning and coding-support tools to support explanation of predictive-analytics concepts, Python/Pandas/NumPy/Scikit-learn code, debugging, and workflow organization. The student is responsible for reviewing, understanding, validating, and explaining the submitted analysis, model choices, evaluation results, interpretations, and business recommendations.

## Dataset
Big Mart Sales Prediction dataset, obtained from Kaggle.
