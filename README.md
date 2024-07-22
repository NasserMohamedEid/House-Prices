# House Prices: Advanced Regression Techniques
## Introduction
In this project, we explore various regression techniques to build a model that can accurately predict house prices. The project involves data preprocessing, feature engineering, feature selection, model training, and evaluation.
## Data Preprocessing

Data preprocessing is crucial for transforming raw data into a format suitable for modeling. The following steps are involved:

- **Handling Missing Values:**
  - **Categorical Features:** Filled with the mode (most frequent value) to address missing values.
  - **Numerical Features:** Filled with the median value to ensure robustness against outliers.

- **Encoding Categorical Variables:**
  - **Ordinal Features:** Utilized label encoding to preserve the ordinal relationship between categories.
  - **Nominal Features:** Applied one-hot encoding to convert categorical variables into a binary matrix.

- **Normalizing Numerical Features:**
  - **Scaling:** Rescaled numerical features to a range between 0 and 1 for uniformity across different features.

- **Handling Outliers:**
  - **Detection and Management:** Identified and addressed outliers in both the target variable and other numerical features to prevent skewed results and improve model performance.

---

## Feature Engineering

Feature engineering involves creating additional features to enhance model performance. This includes:

- **Interaction Features:** Generating new features that capture interactions between existing features.
- **Aggregated Information:** Creating aggregated features to summarize information and capture trends.
- **Transformation of Skewed Features:** Applying transformations to skewed features to improve their distribution.

---

## Feature Selection

Feature selection is performed to improve model performance by reducing overfitting and computational cost. The methods used include:

- **Correlation Analysis:** Retained features with high correlation with the target variable to ensure relevance.
- **Recursive Feature Elimination (RFE):** Used RFE to iteratively remove less important features based on model performance until the desired number of features was achieved.
- **Feature Importance from Tree-based Models:** Utilized feature importance scores from models like Random Forest and Gradient Boosting to select features with the highest impact on the target variable.

---
## Modeling

Various regression models are employed to predict house prices:

- **Linear Regression**
- **GBM**
- **KNN**
- **XGBoost**
- **LightGBM**
- **CatBoost Regressor**
- **Support Vector Regressor (SVR)**

Hyperparameter tuning is performed using GridSearchCV to find the best model parameters.

---
## Evaluation

The models are evaluated using the following metrics:

- **Mean Squared Error (MSE)**
- **R-squared (R²)**

Cross-validation is used to ensure the models generalize well to unseen data.

---
## Conclusion
The project demonstrates the application of various regression techniques for predicting house prices. The best-performing model is identified, and its performance metrics are discussed.
