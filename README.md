# fraud-detection

The general purpose of this project is to develop an insurance fraud detection system which incorporates feature engineering, ML/DL models, hyperparameter tuning and model evaluation techniques. The final model is intended to be deployed on to AWS.

# Project Overview

## Phase I - Data Loading & Cleaning

- Load dataset
- Examine for
-   Data Types
-   Missing Values
-   Feature Distribution
-   Feature Range
-   Potential Outliers
-   Class Imbalances
- Impute or remove missing values
- Use feature engineering to extract new insights from time, history, vehicle type, etc.
- Encode categorical variables
- Scale numeric features with MinMaxScaler

## Phase II - EDA

- Plot fraud vs. non-fraud distributions with histograms and KDE plots
- Use correlation heatmaps to discover feature relationships
- Identify potential outliers in amounts

## Phase III - Model Development & Optimization

- Train the following models with k-fold cross-validation
-   Logistic Regression
-   Decision Trees
-   Random Forests
-   XGBoost
- Train the following DL models with early stopping and learning rate scheduling
-   FFNN
-   FFNN + BN
-   FFNN + Dropout
-   FFNN + BN + Dropout
- Optimize classical ML models with RandomizedSearchCV and BayesSearchCV
- Optimize DL models with Keras Tuner

## Phase IV - Model Evaluation

- Evaluate models with
-   Precision
-   Recall
-   F1-Score
-   AUC-ROC
-   SHAP & LIME

## Phase V - Model Deployment

- Build an API with FastAPI
- Containerize the model with Docker
- Deploy on AWS Lambda

