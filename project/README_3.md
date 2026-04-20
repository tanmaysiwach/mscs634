# MSCS_634_ProjectDeliverable_3

## Classification, Clustering, and Pattern Mining

---

## Dataset Overview

This project uses the Heart Disease Dataset, which includes patient information such as age, cholesterol, blood pressure, and other clinical features. The target variable (`output`) indicates the presence (1) or absence (0) of heart disease.

Data preprocessing from earlier deliverables included handling missing values, removing duplicates, and standardizing features.

---

## Objectives

* Develop and evaluate classification models
* Apply clustering to identify patterns in the data
* Perform association rule mining to uncover relationships
* Interpret results in a practical context

---

## Classification Models

### Models

* Logistic Regression
* Decision Tree Classifier

### Evaluation

Models were assessed using confusion matrix, accuracy, precision, recall, F1-score, and ROC curve.

### Key Findings

Logistic Regression showed stable performance for binary classification. The Decision Tree initially overfit but improved after hyperparameter tuning using GridSearchCV.

### Insight

Classification models can effectively predict heart disease risk based on patient attributes.

---

## Clustering Analysis

### Model

* K-Means Clustering

### Approach

The Elbow Method was used to select the number of clusters, and PCA was applied for visualization.

### Findings

Clusters revealed distinct patient groups, with some segments showing higher risk profiles based on features such as age and cholesterol.

### Insight

Clustering helps identify meaningful patient segments for targeted analysis.

---

## Association Rule Mining

### Method

* Apriori Algorithm

### Metrics

* Support, Confidence, Lift

### Findings

Patterns indicated that combinations of factors, such as higher age and cholesterol, are associated with increased heart disease risk.

### Insight

Association rules provide interpretable relationships between risk factors.

---

## Challenges

* Converting continuous variables into binary format for Apriori
* Addressing overfitting in the Decision Tree model
* Interpreting clusters without predefined labels

---

## Conclusion

This deliverable applied classification, clustering, and association rule mining to extract insights from the dataset. These methods collectively enhance understanding of risk factors and support data-driven decision-making.
