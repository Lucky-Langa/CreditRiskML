# 🏦 ML Loan-Solutions Elite: Predicting Loan Approval  

## 🏆 Problem Statement  
It is a **classification problem** where we must predict whether a loan will be **approved** or **not**, based on structured financial data.  

## 🔍 Best Model Used  
After extensive evaluation, the best-performing model is **RandomizedSearchCV applied to RandomForest**, achieving **99.26% accuracy**.  

## 📊 Models Compared  
- **RandomForest (Tuned with RandomizedSearchCV) ✅**  
- Logistic Regression 📉  
- Decision Tree 🌳  
- Naive Bayes 📊  
- K-Nearest Neighbors (KNN) 🔍  

## ⚙️ Implementation  

### 📚 Libraries Used  
`sklearn` `Matplotlib` `pandas` `seaborn` `NumPy`  

### 🔧 Hyperparameter Tuning with RandomizedSearchCV  
🚀 **Best RandomForest Parameters:**  
- `n_estimators`: **200**  
- `min_samples_split`: **4**  
- `min_samples_leaf`: **16**  
- `max_depth`: **None**  

📈 **Best DecisionTree Parameters:**  
- `max_depth`: **12**  
- `min_samples_split`: **4**  
- `min_samples_leaf`: **2**  
- `max_features`: **None**  
- `criterion`: **gini**  

## 📊 Model Evaluation  
To assess model performance, we analyzed **training accuracy, test accuracy, and cross-validation scores**:  

| Model | Train Accuracy | Test Accuracy | Cross-Validation Score |
|---------|-------------|-------------|-------------|
| **RandomForest (Tuned)** | **100%** | **99.26%** ✅ | **99.59%** |
| Logistic Regression | **86.96%** | **87.31%** | **87.02%** |
| Naive Bayes | **83.02%** | **83.67%** | **82.98%** |
| **DecisionTree (Tuned)** | **100%** | **99.46%** | **99.42%** |
| KNN | **84.00%** | **84.21%** | **83.89%** |

🔍 **Insights:**  
✅ **RandomForest & DecisionTree show near-perfect accuracy**, suggesting **potential overfitting**.  
✅ **Cross-validation results confirm stability**, but complexity should be monitored.  
✅ **Logistic Regression and Naive Bayes offer more generalized predictions** but slightly lower accuracy.  

## 🔎 Feature Importance (RandomForest)  
After training the **best RandomForest model**, the following features contributed the most to loan approval predictions:

| Feature | Importance |
|---------|-------------|
| **Credit Score** | **0.339** |
| **Employment Status** | **0.313** |
| **Loan Amount** | **0.157** |
| **DTI Ratio** | **0.109** |
| **Income** | **0.081** |

✅ **Credit Score** and **Employment Status** have the highest influence on loan approvals, confirming their significance in financial decision-making.

### 🔨 Steps Taken  
✅ **Converting Categorical Data into Numerical Data**  
✅ **Visualizing Feature Relationships**  
✅ **Hyperparameter Tuning with RandomizedSearchCV**  
✅ **Evaluating Model Performance**  
✅ **Analyzing Feature Importance**  

## 🚀 Future Plans  
🔹 **Deployment & Real-time Prediction** 🖥️  
🔹 **Feature Engineering & Selection for Optimization**  
🔹 **Using NLP for Loan Approval Reasons** 📝  

### 🏗 Clone the Repository  
```sh
git clone https://github.com/Lucky-Langa/CreditRiskML.git
