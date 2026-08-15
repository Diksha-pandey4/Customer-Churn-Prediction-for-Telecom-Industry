Customer Churn Prediction for Telecom Industry
📌 Overview

A machine learning classification project that predicts whether a telecom customer is likely to churn (leave the service), using ensemble models and SMOTE for handling class imbalance.

🎯 Problem Statement

Customer churn directly impacts revenue for subscription-based businesses. This project builds a model to proactively identify customers at risk of churning, so retention efforts can be targeted effectively.

🗂️ Dataset
WA_Fn-UseC_-Telco-Customer-Churn.csv — customer demographic, account, and service usage data with a binary Churn target
🛠️ Tech Stack
Python
Pandas, NumPy
Matplotlib, Seaborn — visualization
Scikit-learn — Decision Tree, Random Forest, model evaluation
Imbalanced-learn (SMOTE) — class balancing
Pickle — model serialization
🔍 Approach
Data Cleaning — Removed non-predictive customerID column, handled blank/missing values in TotalCharges
Exploratory Data Analysis — Analyzed numerical feature distributions (histograms, boxplots) and categorical feature counts, plus a correlation heatmap
Encoding — Label-encoded the target and all categorical features, saving encoders for consistent inference later
Handling Class Imbalance — Applied SMOTE to the training set to balance churned vs. non-churned classes
Model Selection — Compared Decision Tree, Random Forest, and XGBoost using 5-fold cross-validation; selected Random Forest as the best performer
Model Evaluation — Assessed final model using Accuracy, Confusion Matrix, and Classification Report on held-out test data
Predictive System — Serialized the trained model and encoders with Pickle for reuse on new customer data
📊 Results
Random Forest outperformed Decision Tree and XGBoost on cross-validated accuracy
Built a reusable inference pipeline that loads the saved model/encoders and predicts churn for new customer records
🚀 How to Run
bash
git clone <repo-link>
cd customer-churn-prediction
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn xgboost
jupyter notebook Customer_Churn_Prediction.ipynb
🔮 Future Improvements
Hyperparameter tuning (GridSearchCV/RandomizedSearchCV) for the Random Forest model
Add feature importance analysis to explain key churn drivers
Deploy as a Streamlit app for interactive churn prediction
👤 Author

Diksha Pandey.
