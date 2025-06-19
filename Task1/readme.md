# 📊 Loan Approval Dataset Analysis  

## 🔍 Overview  
This project analyzes a loan approval dataset to explore applicant features like income, loan amount, and credit score.
The goal is to uncover patterns and relationships that could inform loan approval decisions.  

## 📂 Dataset  

The dataset (`loan_approval_dataset.csv`) : https://www.kaggle.com/datasets/suryadeepthi/loan-approval-dataset

contains **5,000 rows** and **14 columns**, including:  
- Numerical: `Income`, `Loan_Amount`, `Credit_Score`  
- Categorical: `Employment_Status`, `Marital_Status`, `Property_Ownership`  

## 📋 Tasks Performed  

### 📌 **Data Exploration**  
- Displayed first/last 12 rows.  
- Checked data types and missing values.  
- Analyzed statistics (mean, median, standard deviation).  
- Identified most frequent values and unique categories.  

### 🧹 **Data Cleaning**  
- Removed duplicate rows.  
- Filled missing values (mode for categorical, median for numerical).  
- Converted `Credit_Score` to string.  

### 📈 **Feature Engineering**  
- Created **`Income_to_Loan_Ratio`** → Measures repayment capacity.  
- Added **`EMI`** (Equated Monthly Installment) → Assesses financial burden.  

### 📉 **Visualizations**  
- **Boxplot** for `Loan_Amount` (detected outliers).  
- **Histogram** for `Income` (distribution analysis).  
- **Scatterplot** for `Income vs. Loan_Amount` (positive correlation).  
- **PCA** for dimensionality reduction.  
- **Heatmap** for feature correlations.  

## 🔎 **Key Insights**  
- 💰 Higher-income applicants tend to request larger loans.  
- ⚖️ Dataset is balanced across `Employment_Status` categories.  
- 📉 Weak correlations between most numerical features.  
- ✨ New features (`Income_to_Loan_Ratio`, `EMI`) enhance risk assessment.  

## 🛠 **Tools Used**  
![Python](https://img.shields.io/badge/-Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/-Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/-NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/-Scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Matplotlib](https://custom-icon-badges.demolab.com/badge/Matplotlib-71D291?style=for-the-badge&logo=matplotlib)
![Seaborn](https://img.shields.io/badge/-Seaborn-5C8EBC?style=for-the-badge&logo=pypi&logoColor=white)
![Google Colab](https://img.shields.io/badge/Google%20Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=fff)

**Key Libraries**:  

- **Pandas**: Data cleaning, transformation, and analysis.
- **NumPy**: Numerical computations and array operations.
- **Scikit-learn**: PCA implementation and data standardization.
- **Matplotlib**: Foundational plotting for charts and graphs.
- **Seaborn**: Advanced statistical visualizations and heatmaps.

**Development**:  
- **Google Colab** for cloud-based execution and collaboration.

## 🎯 **Conclusion**  
This analysis provides actionable insights for loan approval decisions, highlighting key trends and engineered features for better risk assessment.  
