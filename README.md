# 🌀 Customer Segmentation with K-Means

This project demonstrates how to apply **K-Means clustering** to group customers based on demographic, socioeconomic, and behavioral data.  
The goal is to identify distinct customer segments that could be useful for targeted marketing, product recommendations, or business strategy.

---

## 📖 Project Summary
- Dataset: 2,000 customers with features such as **Age**, **Gender**, **Annual Income**, **Spending Score**, **Profession**, **Work Experience**, and **Family Size**.
- Preprocessing: Selected relevant features and standardized them using `StandardScaler` to improve clustering performance.
- Clustering: Used the **Elbow Method** to determine the optimal number of clusters, then applied **K-Means**.
- Visualization: Created clear plots to show the distribution of clusters and their differences.

---

## 📊 Insights Provided
From this analysis, you can:
- Identify groups of customers with similar spending patterns and income levels.
- Understand the relationship between demographic factors (e.g., age, family size) and spending behavior.
- Detect potential high-value or low-engagement customer segments.
- Use segmentation to adapt marketing strategies for each group.

---

## 🛠 Tools & Libraries
- **Python** – main programming language
- **Pandas / NumPy** – data manipulation
- **Matplotlib / Seaborn** – visualization
- **Scikit-learn** – preprocessing and K-Means implementation

---

## 🔍 Process
1. **Load Data** – Imported `Customers.csv` and reviewed structure and statistics.
2. **Preprocess** – Selected numerical features and standardized them.
3. **Determine Number of Clusters** – Applied the Elbow Method to find the optimal `k`.
4. **Train Model** – Ran K-Means with the chosen number of clusters.
5. **Analyze & Visualize** – Plotted clusters to interpret differences.

---

## 📈 Results
- The Elbow Method indicated that **3 clusters** gave a reasonable starting point.
- Visualization showed some separation between groups based on income and spending score.
- Each cluster represents a different type of customer profile.

### 📏 Model Evaluation
To evaluate the quality of clustering, a **Silhouette Score** was calculated: 0.138
A score closer to **1** indicates well-separated clusters, while values near **0** suggest overlapping groups.  
A score of **0.138** means the clusters in this setup are **weakly separated**.  

**Possible reasons:**
- Features used may not strongly distinguish customer groups.
- Data could benefit from additional feature engineering or dimensionality reduction.

**Next steps for improvement:**
- Test different `k` values to compare scores.
- Try alternative clustering algorithms (e.g., DBSCAN, Agglomerative Clustering).
- Selection to focus on the most relevant variables.

