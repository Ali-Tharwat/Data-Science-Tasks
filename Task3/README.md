# 🛍️ Mall Customer Segmentation Analysis  

## 📊 Overview  
This project segments mall customers into distinct groups using clustering techniques like KMeans, Agglomerative Clustering, GMM, and BIRCH. The goal is to identify customer behavior patterns based on income, spending, and demographics for targeted marketing strategies.  

## 📂 Dataset  

The dataset (`Mall_Customers.csv`) contains **200 entries** with **5 features**, including:  
- **Numerical**: `Age`, `Annual Income (k$)`, `Spending Score (1-100)`  
- **Categorical**: `Gender`  

---

## 🔍 Tasks Performed  

### 🧹 **Data Preparation**  
- Encoded categorical features (`LabelEncoder`).  
- Scaled numerical features for clustering (`StandardScaler`).  
- Applied **PCA** for dimensionality reduction and visualization.  

### 📊 **Clustering Techniques**  
- **KMeans** → Optimal clusters identified using the Elbow Method.  
- **Agglomerative Clustering** → Hierarchical approach for flexible grouping.  
- **Gaussian Mixture Model (GMM)** → Probabilistic clustering for overlapping groups.  
- **BIRCH** → Scalable method for large datasets (though tested here on small data).  

### 📈 **Model Evaluation**  
- **Metrics**: Silhouette Score, Davies-Bouldin Index.  
- **Key Findings**:  
  - ✅ **KMeans** performed best (highest Silhouette Score, clear clusters).  
  - 🔄 **Agglomerative** and **GMM** showed competitive results with slight overlaps.  
  - ⚠️ **BIRCH** struggled with unbalanced clusters on this small dataset.  

---

## 💡 **Key Insights**  
- 🎯 **KMeans** is ideal for spherical, well-separated clusters (e.g., customer segments).  
- 🌐 **GMM** handles overlapping clusters better but requires careful tuning.  
- ⚡ **BIRCH** is efficient for large-scale data but less effective here.  

---

## 🛠️ **Tech Stack**  
![Python](https://img.shields.io/badge/-Python-3776AB?style=for-the-badge&logo=python&logoColor=white) 
![Pandas](https://img.shields.io/badge/-Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white) 
![NumPy](https://img.shields.io/badge/-NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white) 
![Scikit-learn](https://img.shields.io/badge/-Scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white) 
![Matplotlib](https://custom-icon-badges.demolab.com/badge/Matplotlib-71D291?style=for-the-badge&logo=matplotlib)
![Seaborn](https://img.shields.io/badge/-Seaborn-5C8EBC?style=for-the-badge&logo=pypi&logoColor=white)

**Key Libraries**:  
- **Pandas**: Data preprocessing.  
- **NumPy**: Numerical operations.  
- **Scikit-learn**: Clustering algorithms and metrics.  
- **Matplotlib & Seaborn**: Visualizations.  

**Development**:  
- **Google Colab** for cloud-based execution.

---

## 🎯 **Conclusion**  
**KMeans** emerged as the most effective method for this dataset, offering:  
- High interpretability.  
- Clear cluster boundaries.  
- Actionable insights for marketing strategies.  
