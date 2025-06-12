# Land Cover Classification using NDVI Time-Series

## Data Preprocessing and Feature Engineering:
- KNN Imputation: was initially used to fill missing NDVI values.
- Principal Component Analysis (PCA): was applied to denoise the dataset while preserving maximum variance.
- Statistical Feature Engineering: involved deriving meaningful indicators like mean, standard deviation, and temporal statistics from the NDVI time series.
- All processing steps are supported by clear visualizations to aid interpretation and debugging.

## Model Development:
- The core classification model used is Logistic Regression, which performed exceptionally well due to the simplicity and structure of the engineered features.
- Final accuracy achieved: 0.945
- A confusion matrix and other metrics were also evaluated.

## Alternate Experiments:
- More complex pipelines involving simple median imputation, complex denoising techniques, and advanced feature engineering were also tried.
- However, these led to reduced performance (accuracy ~0.88), likely due to:
  - Overfitting on overly transformed features
  - Loss of signal from excessive denoising
  - Feature redundancy that confused the simpler classifier

## Key Learnings:
- Simple preprocessing + Logistic Regression outperformed more complex methods, validating the importance of understanding data over blindly applying sophisticated models.
- PCA worked effectively in reducing noise from temporal NDVI data.
- Feature selection and interpretability are crucial in classification tasks with time-series data.

This project uses Python with libraries like `pandas`, `scikit-learn`, `seaborn`, and `matplotlib`. The notebook includes all data processing steps, visualizations, model training, and performance evaluation.

📌 Maintained by Deepika Yadav (deepikayadaviit@gmail.com)
I am open for suggestions and feedbacks!!!
