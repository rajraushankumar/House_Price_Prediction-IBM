# House Price Prediction Using Machine Learning

## AICTE | IBM SkillsBuild Academic Internship – Data Analytics with AI

**Project Title:** House Price Prediction Using Machine Learning  
**Author:** Rajraushan Kumar  
**Internship:** AICTE | IBM SkillsBuild Academic Internship – Data Analytics with AI | BharatCares  
**Dataset:** Kaggle – House Prices: Advanced Regression Techniques

---

## 1. Project Overview

This project develops a machine learning system to predict residential house prices using the Kaggle House Prices dataset.

The project follows an end-to-end data science workflow including data analysis, preprocessing, exploratory data analysis, machine learning, model evaluation, feature importance analysis, and model saving.

Two regression models were trained and compared:

1. Linear Regression
2. Random Forest Regressor

---

## 2. Problem Statement

House prices depend on several factors such as house quality, living area, number of rooms, garage features, year built, neighborhood, and other property characteristics.

The objective of this project is to use these features to predict the final house sale price.

**Target Variable:** `SalePrice`

---

## 3. Objectives

- Analyze the house price dataset.
- Identify important features.
- Handle missing values.
- Perform exploratory data analysis.
- Prepare data for machine learning.
- Train regression models.
- Evaluate model performance.
- Analyze feature importance.
- Save the trained machine learning model.

---

## 4. Dataset

**Dataset:** House Prices: Advanced Regression Techniques  
**Source:** Kaggle

The dataset contains information about residential properties and their sale prices.

The target variable used for prediction is:

```text
SalePrice

7. Exploratory Data Analysis

The project includes analysis of:

Sale price distribution
Correlation between numerical variables
Overall quality versus sale price
Living area versus sale price
Actual versus predicted prices
Prediction errors
Feature importance
Generated Visualizations

The following visualizations are saved in the reports/ folder:

saleprice_distribution.png
correlation_heatmap.png
overall_quality_vs_price.png
living_area_vs_price.png
actual_vs_predicted.png
prediction_errors.png
feature_importance.png
8. Data Preprocessing

Numerical and categorical features were processed using a Scikit-learn preprocessing pipeline.

Numerical Features

Missing numerical values were handled using median imputation.

Categorical Features

Missing categorical values were handled using the most frequent value and categorical variables were converted using One-Hot Encoding.

A ColumnTransformer and Pipeline were used to maintain a consistent preprocessing workflow.

9. Machine Learning Models
Linear Regression

Linear Regression was used as a baseline regression model.

Random Forest Regressor

Random Forest Regressor was used as the main tree-based regression model.

Configuration:

n_estimators = 300
random_state = 42
n_jobs = -1
10. Model Performance

The models were evaluated using:

MAE – Mean Absolute Error
RMSE – Root Mean Squared Error
R² – Coefficient of Determination
Model	MAE	RMSE	R²
Linear Regression	$20,485.66	$31,327.80	0.8720
Random Forest Regressor	$17,465.29	$28,554.98	0.8937

The Random Forest Regressor achieved an R² of 0.8937 on the project's test set and was saved as the final model.

11. Model Saving

The trained Random Forest model was saved using Joblib.

models/house_price_prediction_model.pkl

The saved model was also loaded again and verified successfully for prediction.

12. Project Structure
House_Price_Prediction_IBM/
│
├── data/
│   └── train.csv
│
├── notebooks/
│   └── Rajraushan_House_Price_Prediction_IBM.ipynb
│
├── models/
│   └── house_price_prediction_model.pkl
│
├── reports/
│   ├── saleprice_distribution.png
│   ├── correlation_heatmap.png
│   ├── overall_quality_vs_price.png
│   ├── living_area_vs_price.png
│   ├── actual_vs_predicted.png
│   ├── prediction_errors.png
│   └── feature_importance.png
│
├── requirements.txt
├── README.md
└── .venv/
13. How to Run
Step 1: Open the project in VS Code

Open the House_Price_Prediction_IBM folder in VS Code.

Step 2: Create a virtual environment
python -m venv .venv
Step 3: Activate the environment

For Windows:

.venv\Scripts\activate
Step 4: Install dependencies
pip install -r requirements.txt
Step 5: Open the notebook

Open:

notebooks/Rajraushan_House_Price_Prediction_IBM.ipynb
Step 6: Select the Python kernel

Select the project's .venv Python environment.

Step 7: Run the notebook

Run all cells from beginning to end.

14. Key Findings
Overall house quality is an important factor related to sale price.
Living area is an important feature for house price prediction.
Both numerical and categorical features contribute to the model.
Random Forest Regressor achieved an R² of 0.8937 on the test set.
The trained model was successfully saved and loaded using Joblib.
15. Future Improvements

Possible future improvements include:

Hyperparameter tuning
Cross-validation
Feature engineering
Outlier treatment
Target transformation
Testing additional regression algorithms
Deploying the model as a web application
Creating an interactive prediction interface
16. Conclusion

This project demonstrates an end-to-end machine learning workflow for house price prediction.

It covers data analysis, preprocessing, visualization, model training, evaluation, feature importance analysis, and model persistence.

The project demonstrates how machine learning can be applied to housing data to predict sale prices using multiple property-related features.

17. Author

Rajraushan Kumar

BCA – Data Science & AI
Gopal Narayan Singh University

18. Internship

This project was developed as part of:

AICTE | IBM SkillsBuild Academic Internship – Data Analytics with AI | BharatCares