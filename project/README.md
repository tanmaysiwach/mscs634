# Heart Disease Data Mining Project

## Dataset Summary

This project uses the **UCI Heart Disease Dataset**, which contains medical information used to determine whether a patient has heart disease. The dataset includes attributes such as age, cholesterol level, blood pressure, chest pain type, and maximum heart rate. The target variable **`output`** indicates whether heart disease is present (1) or not (0).

## Key Insights

Initial exploratory analysis revealed several patterns:

* Age and cholesterol levels appear related to heart disease risk.
* Patients with certain chest pain types show a higher likelihood of heart disease.
* Maximum heart rate and exercise-induced angina may influence heart disease prediction.

These insights suggest that several medical features may be useful for building predictive models.

## Data Cleaning and Exploration Steps

The following steps were performed to prepare the dataset:

* Loaded the dataset using **Pandas** and inspected its structure.
* Checked for missing values and duplicates.
* Removed duplicate records and verified data types.
* Conducted exploratory data analysis (EDA) using **Matplotlib** and **Seaborn** to examine feature distributions, detect outliers, and explore relationships between variables.

## Challenges and Solutions

One challenge was ensuring the dataset contained consistent and clean data for analysis. Duplicate entries were identified and removed to prevent bias in the analysis. Additionally, exploratory visualizations were used to better understand feature distributions and detect potential outliers, helping guide further analysis and modeling steps.
