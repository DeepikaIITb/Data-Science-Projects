This was all about dealing with imbalanced data and classification score of 1.0

# Classification Model with Preprocessing & GridSearchCV
This project demonstrates a full classification pipeline using scikit-learn. It includes handling skewed data, removing outliers, scaling features, balancing imbalanced classes using SMOTE, and tuning hyperparameters with GridSearchCV. Multiple models are evaluated including Logistic Regression, Random Forest, Decision Tree, KNN, and SVC.

Features
- Log transformation for skewed features
- Outlier removal
- Feature scaling
- SMOTE for class imbalance
- GridSearchCV with cross-validation
- Classification metrics: accuracy, precision, recall, F1

Getting Started
1. Clone the repo  
2. Install dependencies (`pip install -r requirements.txt`)  
3. Run the notebook and explore the pipeline

Sample Result
KNN gave the most realistic score (~0.978); others showed 1.0 due to possible overfitting. Pipelines are recommended to avoid data leakage.

---

📌 Maintained by Deepika Yadav (deepikayadaviit@gmail.com)
