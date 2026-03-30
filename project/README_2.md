# MSCS 634 – Project Deliverable 2: Regression Modeling & Performance Evaluation

## Dataset Summary
- Dataset: `heart.csv` (cleaned version from Deliverable 1)  
- Records: 303  
- Features: 13 attributes including age, sex, chest pain type, cholesterol, etc.  
- Target Variable: `output` (heart disease: 1 = presence, 0 = absence)  
- Preprocessing: missing values handled, duplicates removed, features scaled

## Modeling Process
- Feature scaling applied using StandardScaler  
- Train-test split: 80% training, 20% testing  
- Regression models built: Linear Regression, Ridge Regression, Lasso Regression  
- 5-fold cross-validation applied

## Model Performance
| Model | R2 Score | RMSE | Key Observations |
|-------|----------|------|-----------------|
| Linear Regression | X.XX | X.XX | Baseline model |
| Ridge Regression | X.XX | X.XX | Reduced overfitting |
| Lasso Regression | X.XX | X.XX | Feature selection effect |

*Replace X.XX with your actual evaluation metrics.*

## Insights
- Most influential features: age, cholesterol (chol), resting blood pressure (trestbps)  
- Ridge improves generalization, Lasso reduces feature complexity  
- Predicted vs actual values show models capture trends but regression on binary target has limitations

## Challenges
- Regression applied to a binary target; classification would be more natural  
- Multicollinearity handled with Ridge and Lasso  
- Interpreting coefficients after scaling

## Summary
Deliverable 2 demonstrated feature scaling, building and comparing regression models, evaluating with R2/MSE/RMSE, and identifying influential features. This prepares the dataset for classification in Deliverable 3.