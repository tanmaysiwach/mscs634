# 🛒 Association Rule Mining باستخدام Apriori و FP-Growth

## 📌 Overview
This lab explores **association rule mining techniques** using the Apriori and FP-Growth algorithms. The goal is to analyze transactional retail data, discover frequent itemsets, and generate meaningful association rules that reveal hidden patterns in customer purchasing behavior.

---

## 📂 Dataset
The dataset used in this lab is a transactional retail dataset containing the following columns:

- `Invoice` – Transaction ID  
- `StockCode` – Product code  
- `Description` – Product name  
- `Quantity` – Number of items purchased  
- `InvoiceDate` – Date of transaction  
- `Price` – Price per item  
- `Customer ID` – Unique customer identifier  
- `Country` – Customer location  

---

## ⚙️ Data Preprocessing
The following cleaning steps were applied:

- Removed missing values in `Invoice` and `Description`
- Filtered out cancelled transactions (Invoice starting with 'C')
- Removed rows with non-positive quantities
- Converted data into a **transaction matrix (basket format)**
- Transformed quantities into binary values (0/1)

---

## 📊 Exploratory Data Analysis
Visualizations were created using **Seaborn** to better understand the dataset:

- Bar plot of top 10 most frequently purchased items
- Heatmap showing item co-occurrence and correlations

---

## 🔍 Algorithms Used

### 1. Apriori Algorithm
- Generates frequent itemsets using a candidate generation approach
- Requires multiple scans of the dataset
- Support threshold: `0.01`

### 2. FP-Growth Algorithm
- Uses a compact tree structure (FP-tree)
- More efficient than Apriori for large datasets
- Same support threshold for fair comparison

---

## 📈 Association Rules
Association rules were generated using:

- **Metric:** Confidence  
- **Minimum Threshold:** 0.5  

### Key Metrics:
- **Support** – Frequency of itemset occurrence  
- **Confidence** – Likelihood of co-occurrence  
- **Lift** – Strength of association (>1 indicates strong relationship)  

---

## 📊 Visualizations
- Bar plots for top frequent itemsets
- Scatter plot of **Confidence vs Lift**
  - Helps identify strong and meaningful rules

---

## ⚖️ Comparison: Apriori vs FP-Growth

| Feature        | Apriori              | FP-Growth           |
|----------------|---------------------|---------------------|
| Speed          | Slower              | Faster              |
| Method         | Candidate generation| Tree-based (FP-tree)|
| Scalability    | Limited             | High                |
| Memory Usage   | Higher              | More efficient      |

### ✅ Conclusion:
FP-Growth performed better in terms of execution time and scalability, especially for large datasets.

---

## ⚠️ Challenges Faced
- Large dataset caused slow execution (Apriori)
- Sparse data led to limited frequent itemsets
- Memory usage issues during transformation
- Managed environemnt, had issues with pip and installing seaborn and other libs

### ✅ Solutions
- Reduced support threshold
- Filtered dataset when necessary
- Optimized transaction matrix creation

---

## 💡 Key Insights
- Certain products are frequently purchased together
- High lift values indicate strong product associations
- These insights can be used for:
  - Product recommendations
  - Cross-selling strategies
  - Store layout optimization