# Wine Classification using KNN and Radius Neighbors

## 📌 Purpose of the Lab

The purpose of this lab is to explore and compare the performance of two instance-based learning algorithms: **K-Nearest Neighbors (KNN)** and **Radius Neighbors (RNN)** using the Wine dataset from sklearn.

By experimenting with different parameter values (k for KNN and radius for RNN), this lab aims to demonstrate how model performance is affected by these choices and to identify optimal configurations for classification accuracy.

---

## 📊 Key Insights and Observations

* **KNN Performance:**

  * Smaller values of k (e.g., k=1) tend to produce higher variance and may overfit the data.
  * Moderate values of k (e.g., k=5 or k=11) generally provide better and more stable accuracy.
  * Larger k values smooth decision boundaries but may slightly reduce accuracy due to underfitting.

* **RNN Performance:**

  * The choice of radius significantly impacts performance.
  * Smaller radius values may result in some points having no neighbors, reducing accuracy.
  * Larger radius values include more neighbors, which can improve coverage but may lower precision.

* **Overall Comparison:**

  * KNN provided more consistent and reliable results across different parameter values.
  * RNN was more sensitive to parameter selection and required careful tuning.

---

## ⚠️ Challenges and Decisions

* **Feature Scaling:**

  * Distance-based algorithms like KNN and RNN are sensitive to feature scales.
  * Standardization (using `StandardScaler`) was necessary to ensure fair distance calculations.

* **Choosing Radius Values:**

  * Initial radius values were too large relative to scaled data.
  * Adjustments were needed to avoid cases where all or no neighbors were selected.

* **Handling Outliers in RNN:**

  * Some test points had no neighbors within the specified radius.
  * The `outlier_label='most_frequent'` parameter was used to handle such cases.

* **Parameter Selection:**

  * Selecting appropriate k and radius values required experimentation and observation of trends rather than relying on a single configuration.

---

## ✅ Conclusion

This lab highlights the importance of parameter tuning in distance-based models. While both KNN and RNN can be effective, KNN generally offers more stable performance, whereas RNN can be useful in scenarios where neighborhood size should vary dynamically based on distance.

---
