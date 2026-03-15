# Data Visualization and Preprocessing Lab

## Purpose
The purpose of this lab is to apply data visualization, preprocessing, and statistical analysis techniques to a dataset. The lab focuses on exploring the data, cleaning it, handling missing values and outliers, reducing and scaling the data, and performing basic statistical analyses. These steps prepare the dataset for more advanced data mining and machine learning tasks.

## Key Insights
From visualizations and statistical analysis:

- **Age Distribution:** Most subjects are between 40–60 years old, highlighting the target age range for analysis.  
- **Scatter and Box Plots:** Cholesterol levels and chest pain type appear related to heart disease presence.  
- **Outliers:** Some extreme cholesterol and blood pressure values were identified and removed to reduce skew.  
- **Statistical Measures:** Central tendency (mean, median, mode) and dispersion (range, variance, standard deviation, IQR) provided insight into data spread and variability.  
- **Correlation Analysis:** Numeric features such as age, maximum heart rate, and cholesterol show meaningful correlations with heart disease outcomes.

These insights guided decisions for feature selection, preprocessing, and further modeling.

## Challenges and Decisions
- **Missing Values:** Detected in some columns; handled using mean imputation to maintain dataset size.  
- **Outliers:** Extreme values in numerical columns were removed using IQR to prevent bias in analysis.  
- **Scaling:** Applied Min-Max scaling to standardize numerical features for consistent analysis.  
- **Column Selection:** Less relevant columns were dropped to simplify the dataset and focus on key predictors.  

Overall, careful preprocessing and exploratory analysis ensured a clean, reliable dataset suitable for further modeling.