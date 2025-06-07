# Linear Regression for EV Sales Forecasting
This project demonstrates a basic yet insightful implementation of Linear Regression for forecasting Electric Vehicle (EV) sales. The workflow covers data preprocessing, handling missing values, feature scaling, and applying regression with performance evaluation.

Data Preprocessing
1. Handling Missing Values:
    Columns or rows containing NaN values were handled using either removal or imputation techniques to ensure model compatibility.
2. Feature Scaling:
    Applied StandardScaler to normalize features before fitting the linear regression model. This is crucial when the feature values vary widely.

Regression Model Applied
1. Linear Regression:
    A baseline regression algorithm used to model the relationship between input features and EV sales. This helps understand linear trends in the data.
2. Steps included:
    Splitting the data into train and test sets
    Scaling the features
    Fitting the linear model
    Predicting test set results
    Evaluating model performance

Model Evaluation
1. Model performance was evaluated using:
    Mean Squared Error (MSE): Measures average squared difference between actual and predicted values.
    R² Score: Indicates how well the independent variables explain the variation in the target variable.
2. Current Results:
    MSE: ~1.717
    R² Score: ~0.836

Key Learnings
  Preprocessing missing values is essential for Linear Regression models.
  Feature scaling significantly affects model performance.
  Even simple models like Linear Regression can achieve high accuracy with proper data treatment.
  A good R² score (~0.83) shows promising predictive power for sales forecasting.

Technologies Used
Python 🐍
Pandas for data manipulation
Scikit-learn for modeling and preprocessing
NumPy, Matplotlib (optional) for support and visualization

Next Steps (optional ideas)
  Try Polynomial Regression to capture non-linear trends.
  Compare with tree-based models like Random Forest or Gradient Boosting.
  Apply GridSearchCV for hyperparameter tuning.
  Visualize predictions vs actual sales.

📌 Maintained by Deepika Yadav 
📧 deepikayadaviit@gmail.com

