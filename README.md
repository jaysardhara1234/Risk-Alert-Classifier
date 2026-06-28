# 💳 Risk Alert Classifier using Machine Learning

> An end-to-end Machine Learning classification project that predicts whether a customer is **High Risk** or **Low Risk** based on financial and behavioral attributes.

![Python](https://img.shields.io/badge/Python-3.13-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-orange?logo=pandas)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-f7931e?logo=scikitlearn)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-blue)
![Seaborn](https://img.shields.io/badge/Seaborn-EDA-green)
![Status](https://img.shields.io/badge/Project-Completed-success)

---

# 📌 Project Overview

Financial institutions evaluate customers before approving loans or credit cards. Incorrectly identifying high-risk customers can lead to financial losses, while rejecting trustworthy customers affects customer satisfaction.

This project develops a Machine Learning classification model that predicts customer risk status using demographic, financial, and behavioral features.

The project follows a complete ML workflow including:

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Missing Value Imputation
- Feature Scaling
- Model Building
- Model Evaluation
- Model Comparison

---

# 🎯 Objective

Build a classification model capable of accurately predicting whether a customer belongs to the **High Risk** or **Low Risk** category.

---

# 📂 Dataset Information

The dataset contains customer-related financial and behavioral information including:

- Annual Income
- Credit Score
- Credit Utilization Ratio
- Missed Payments
- Average Late Payment Days
- Cash Advance Count
- Complaints
- Failed Login Attempts
- Debt Balance
- Gender
- Region
- Employment Type
- Risk Status (Target)

---

# 🛠️ Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-Learn

---

# 📊 Exploratory Data Analysis (EDA)

The following analyses were performed:

### ✅ Univariate Analysis

- Distribution Plots
- Count Plots
- Box Plots

### ✅ Bivariate Analysis

- Numerical Features vs Risk Status
- Categorical Features vs Risk Status
- Percentage Distribution Analysis

### ✅ Multivariate Analysis

- Correlation Heatmap

### Key Findings

- Credit Score showed a strong negative relationship with customer risk.
- Missed Payments and Average Late Payment Days were strongly associated with High Risk customers.
- Credit Utilization Ratio increased significantly for risky customers.
- Gender had minimal influence on risk classification.
- Employment Type showed a stronger relationship with customer risk.

---

# 🧹 Data Preprocessing

The following preprocessing steps were performed:

- Removed irrelevant features
- Handled missing values
- KNN Imputation for numerical variables
- Most Frequent Imputation for categorical variables
- One-Hot Encoding
- Standard Scaling
- Train-Test Split

---

# ⚙️ Feature Engineering

The following domain-based features were created:

- Debt-to-Income Ratio
- Payment Risk
- Income After Debt

These features were evaluated to determine whether they improved model performance.

---

# 🤖 Machine Learning Models

The following classification algorithms were implemented:

- Logistic Regression
- Logistic Regression with SMOTE
- Decision Tree Classifier
- Random Forest Classifier

---

# 📈 Model Performance

| Model | Precision | Recall | F1 Score | Mean CV F1 |
|--------|----------:|-------:|----------:|-----------:|
| Logistic Regression | **1.000** | **0.981** | **0.991** | **0.983** |
| Logistic Regression + SMOTE | 0.981 | 0.981 | 0.981 | 0.976 |
| Decision Tree | 0.971 | 0.935 | 0.953 | 0.941 |
| Random Forest | 1.000 | 0.954 | 0.976 | 0.976 |

---

# 🏆 Best Model

**Logistic Regression** achieved the highest overall performance.

### Performance

- Precision : **100%**
- Recall : **98.15%**
- F1 Score : **99.07%**
- Mean Stratified Cross Validation F1 : **98.32%**

The model correctly classified almost every customer while producing no false positive predictions.

---

# 📌 Model Comparison

### Logistic Regression

✅ Best overall performance

✅ Highest Cross Validation Score

✅ Highest Recall

✅ No False Positives

---

### Logistic Regression with SMOTE

- SMOTE was applied to address class imbalance.
- Performance did not improve.
- Slight decrease in Precision and F1 Score was observed.
- Baseline Logistic Regression remained superior.

---

### Decision Tree

- Produced strong performance.
- Missed more High Risk customers compared to Logistic Regression.
- Lower Recall and F1 Score.

---

### Random Forest

- Excellent classification performance.
- Perfect Precision.
- Slightly lower Recall than Logistic Regression.

---

# 📊 Evaluation Metrics

The models were evaluated using:

- Precision
- Recall
- F1 Score
- Stratified Cross Validation
- Confusion Matrix

Since the dataset was moderately imbalanced, F1 Score, Precision, and Recall were prioritized over Accuracy.

---

# 💡 Key Insights

- Credit Score is one of the strongest predictors of customer risk.
- Missed Payments significantly increase customer risk.
- Late Payment Days show a strong positive relationship with risk.
- Employment Type influences customer risk more than Gender.
- SMOTE did not improve performance for this dataset.
- Logistic Regression outperformed more complex models despite its simplicity.

---

# 📁 Project Structure

```
Risk Alert Classifier/
│
├── Risk_Alert_Classifier.ipynb
├── Risk_Alert_Classifier_Dataset.csv
├── README.md
```

---

# 🚀 Future Improvements

- Hyperparameter tuning using GridSearchCV or RandomizedSearchCV
- Feature selection techniques
- Probability threshold optimization
- Model deployment using Flask or FastAPI
- Interactive dashboard using Streamlit
- Testing on a real-world financial dataset

---

# 🎓 Learning Outcomes

Through this project, I gained hands-on experience in:

- Exploratory Data Analysis
- Data Cleaning
- Missing Value Imputation
- Feature Engineering
- Feature Scaling
- Machine Learning Classification
- Model Evaluation
- Cross Validation
- Handling Imbalanced Data
- Comparing Multiple Classification Models

---

⭐ If you found this project useful, consider giving it a star!
