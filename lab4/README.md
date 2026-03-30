# MSCS 634 Lab 4: Regression Techniques and Regularization

## Overview

This lab explores different regression models using the Diabetes dataset. The goal is to understand how model complexity and regularization affect performance and overfitting.

The models implemented include Simple Linear Regression, Multiple Regression, Polynomial Regression, Ridge Regression, and Lasso Regression.

## Dataset

The Diabetes dataset from sklearn contains 442 samples with 10 features such as age, BMI, and blood pressure. The target variable represents disease progression.

## Methodology

Data was loaded and explored using basic statistics and visualizations. No missing values were found.

Simple Linear Regression used BMI as the only feature and showed limited performance.

Multiple Regression used all features and significantly improved prediction accuracy.

Polynomial Regression added non-linear relationships and slightly improved results but introduced risk of overfitting at higher degrees.

Ridge and Lasso Regression were applied to reduce overfitting. Ridge shrinks coefficients, while Lasso can remove less important features entirely.

## Evaluation Metrics

Models were evaluated using:

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)
* R-squared (R²)

## Key Insights

Using multiple features improves model performance compared to a single feature. Increasing model complexity can help but may lead to overfitting. Regularization techniques like Ridge and Lasso help control this and improve generalization. Lasso is especially useful for feature selection.

## Challenges

Some challenges included choosing the right polynomial degree and selecting appropriate alpha values for regularization.

## Conclusion

This lab demonstrated how different regression techniques perform and highlighted the importance of balancing model complexity and generalization.
