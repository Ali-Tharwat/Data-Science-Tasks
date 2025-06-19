# 📊 Employee Attrition Prediction  

## 🔍 Overview  
This project predicts employee attrition using machine learning models trained on features like job satisfaction, salary, and tenure. The goal is to identify employees at risk of leaving and evaluate model performance.  

## 📂 Dataset  

The dataset (`employee_attrition_dataset.csv`) :  
#### 🔗Link : [![Kaggle](https://img.shields.io/badge/-Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)](https://www.kaggle.com/datasets/ziya07/employee-attrition-prediction-dataset/data) 
contains **1000 entries** with **26 features**, including:  
- **Numerical**: `Age`, `MonthlyIncome`, `YearsAtCompany`  
- **Categorical**: `Department`, `JobRole`, `Attrition` (target)  

---

## 📋 Tasks Performed  

### 🛠 **Data Preparation**  
- Encoded categorical features (`LabelEncoder`).  
- Split data into **75% train** and **25% test** sets.  
- Scaled features for neural networks (`StandardScaler`).  

### 🤖 **Machine Learning Models**  
- **K-Nearest Neighbors (KNN)** → Balanced precision/recall.  
- **Naive Bayes** → High accuracy but biased to majority class.  
- **Decision Tree** → Captured true positives (21% recall).  
- **Support Vector Machine (SVM)** → High accuracy but zero attrition predictions.
- **Random Forest** → High accuracy but zero attrition predictions.
- **Deep Learning (MLP)** → 3-layer neural network.  

### 📊 **Model Evaluation**  
- **Metrics**: Accuracy, Precision, Recall, Confusion Matrix.  
- **Key Finding**:  
  - 🎯 **KNN** performed best (82% accuracy, 25% precision).  
  - ⚠️ Most models (SVM, RF, MLP) failed to predict attrition cases (0% recall).  

---

## 🔎 **Key Insights**  
- ⚖️ **Class Imbalance**: Models favored majority class (no attrition).  
- 💡 **Decision Tree** was the only model with non-zero recall (21%).  
- 📉 **KNN** struck the best balance between accuracy and actionable predictions.  

---

## 🛠 **Tools Used**  
![Python](https://img.shields.io/badge/-Python-3776AB?style=for-the-badge&logo=python&logoColor=white) 
![Pandas](https://img.shields.io/badge/-Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white) 
![Scikit-learn](https://img.shields.io/badge/-Scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white) 
![TensorFlow](https://img.shields.io/badge/-TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white) 
![Keras](https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=Keras&logoColor=white)
![Google Colab](https://img.shields.io/badge/Google%20Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=fff)  

**Key Libraries**:  
- **Pandas**: Data preprocessing.  
- **Scikit-learn**: KNN, Naive Bayes, Decision Tree , SVM, Random Forest.  
- **TensorFlow/Keras**: Deep learning model (MLP).
  
**Development**:  
- **Google Colab** for cloud-based execution.  

---

## 🏁 **Conclusion**  
While most models achieved high accuracy,

**KNN** emerged as the most practical for real-world attrition prediction due to its ability to identify true positives.  
