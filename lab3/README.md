# Wine Clustering using K-Means and K-Medoids

## Purpose of the Lab
The purpose of this lab is to explore unsupervised learning techniques by applying **K-Means** and **K-Medoids** clustering algorithms to the Wine dataset from sklearn.  

The goal is to understand how clustering algorithms group similar data points without using class labels, and to evaluate their performance using metrics such as **Silhouette Score** and **Adjusted Rand Index (ARI)**.

---

## Key Insights and Observations

- **K-Means Results:**
  - Produced well-separated and compact clusters.
  - Achieved a relatively high Silhouette Score, indicating strong cluster cohesion and separation.
  - Performed efficiently and consistently across the dataset.

- **K-Medoids Results:**
  - Generated clusters that were slightly less uniform but more robust to noise and outliers.
  - Medoids (actual data points) made cluster centers more interpretable.
  - Performance was comparable but slightly lower or more variable than K-Means in terms of Silhouette Score.

- **Comparison:**
  - K-Means generally performed better in terms of cluster compactness.
  - K-Medoids showed advantages in handling potential outliers and irregular cluster shapes.
  - ARI scores indicated how closely clustering aligned with actual class labels, with both methods showing reasonable agreement.

---

## Challenges and Decisions

- **Library Installation Issue:**
  - Encountered a `ModuleNotFoundError` for `sklearn_extra` when implementing K-Medoids.
  - Resolved by either installing the package or implementing a custom K-Medoids algorithm.

- **Feature Scaling:**
  - Standardization using z-score normalization was necessary because clustering algorithms are sensitive to feature magnitude.

- **Visualization:**
  - PCA was used to reduce data to 2D for visualization purposes while preserving as much variance as possible.

- **Parameter Selection:**
  - The number of clusters (k=3) was chosen based on prior knowledge of the dataset.
  - Care was taken to ensure fair comparison by using the same scaled dataset for both algorithms.

---

## Conclusion

This lab demonstrates how clustering algorithms can uncover structure in data without supervision.  
K-Means is efficient and works well for compact clusters, while K-Medoids provides robustness and interpretability.  

Choosing between them depends on dataset characteristics, such as the presence of outliers and the desired level of interpretability.