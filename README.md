# 📊 Customer Churn Prediction using Machine Learning

## 📌 Project Description
Customer churn prediction is a supervised machine learning project aimed at identifying whether a customer is likely to discontinue a service.  
This project uses the **Telco Customer Churn Dataset** to build an end-to-end machine learning pipeline, starting from raw data preprocessing to building a predictive system.

The project includes:
- Data cleaning and preprocessing
- Exploratory Data Analysis (EDA)
- Handling class imbalance using SMOTE
- Training and comparing multiple ML models
- Selecting the best model
- Saving and loading the trained model
- Making predictions on new customer data


## 🎯 Objective
- Predict customer churn accurately
- Understand factors influencing customer churn
- Compare different machine learning models
- Build a reusable churn prediction system


## 📂 Dataset Information
- **Dataset:** Telco Customer Churn Dataset
- **Total Records:** 7043
- **Target Variable:** `Churn`
  - `1` → Customer churned
  - `0` → Customer retained


## 🛠️ Technologies & Libraries Used
- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn (SMOTE)
- Pickle
- XGBoost
- Random Forest Classifier
- Decision Tree

## 🔁 Project Workflow

### 1️⃣ Data Loading
- CSV file loaded using Pandas
- Dataset shape and structure explored

### 2️⃣ Data Cleaning
- Dropped unnecessary column (`customerID`)
- Converted `TotalCharges` from string to numeric
- Handled missing and blank values

### 3️⃣ Exploratory Data Analysis (EDA)
- Distribution analysis using histograms
- Outlier detection using box plots
- Correlation analysis using heatmaps
- Count plots for categorical features

### 4️⃣ Target Encoding
- Converted `Churn` column:
  - `Yes → 1`
  - `No → 0`

### 5️⃣ Feature Encoding
- Applied **Label Encoding** on categorical variables
- Saved encoders using Pickle for future predictions

### 6️⃣ Handling Class Imbalance
- Used **SMOTE (Synthetic Minority Over-sampling Technique)**
- Balanced churn and non-churn classes in training data

### 7️⃣ Train-Test Split
- Dataset split into 80% training and 20% testing data


## 🤖 Machine Learning Models Used

| Model | Description |
|-----|------------|
| Decision Tree Classifier | Rule-based model |
| Random Forest Classifier | Ensemble learning model |
| XGBoost Random Forest | Boosted ensemble model |


## 📊 Model Evaluation
- 5-fold cross-validation performed
- Evaluation metrics used:
  - Accuracy Score
  - Confusion Matrix
  - Classification Report (Precision, Recall, F1-score)

### ✅ Best Model Selected
**Random Forest Classifier**  
Chosen due to better performance and generalization.


## 📌 How to Run the Project

1. Clone or download the project
2. Install required libraries
3. Open the google collab Notebook
4. Run cells sequentially
5. Train models and evaluate results
6. Use the predictive system for new customer data


## 👩‍💻 Author
**Diksha Pandey**  
Machine Learning Project

## 🏁 Conclusion
This project demonstrates a complete machine learning pipeline for customer churn prediction.  

