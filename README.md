# House Price Prediction Using Machine Learning

## Project Overview

This project focuses on predicting residential house prices using Machine Learning techniques.

The project uses the **House Prices: Advanced Regression Techniques** dataset from Kaggle. The target variable is `SalePrice`, and the dataset contains various numerical and categorical features related to residential properties.

Two Machine Learning models were developed and compared:

- Linear Regression
- Random Forest Regressor

After evaluation, the Random Forest Regressor achieved better performance and was saved as the final trained model.

---

## Internship Information

- **Program:** AICTE | IBM SkillsBuild Data Analytics with AI Internship 2026
- **Organization:** BharatCares in association with AICTE and IBM
- **Project:** House Price Prediction Using Machine Learning
- **Student:** Rajraushan Kumar
- **Program:** BCA – Data Science & AI
- **University:** Gopal Narayan Singh University
- **Internship Duration:** 17 August 2026 – 30 September 2026

---

## Problem Statement

House prices depend on several factors such as the overall quality of the property, living area, basement area, garage characteristics, location-related features, and construction year.

The objective of this project is to build a Machine Learning model that can learn from historical housing data and predict the sale price of residential properties.

---

## Objectives

- Analyze the house price dataset.
- Perform Exploratory Data Analysis (EDA).
- Handle missing values.
- Preprocess numerical and categorical features.
- Train Machine Learning regression models.
- Compare model performance using evaluation metrics.
- Identify important features affecting house prices.
- Save the trained Machine Learning model for future use.

---

## Dataset

The dataset used in this project is:

**House Prices: Advanced Regression Techniques**

Dataset source:

https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data

The training dataset contains:

- **1,460 records**
- **81 columns**
- **80 input features**
- **1 target variable**

### Target Variable

`SalePrice`

The target variable represents the final sale price of each residential property.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
- Joblib
- OpenPyXL

---

## Machine Learning Models

### 1. Linear Regression

Linear Regression was used as a baseline regression model.

### 2. Random Forest Regressor

Random Forest Regressor was used as the main Machine Learning model.

Model configuration:

- Number of trees: 300
- Random state: 42
- `n_jobs = -1`

---

## Data Preprocessing

The following preprocessing steps were performed:

1. Loaded the dataset using Pandas.
2. Inspected the dataset structure.
3. Checked missing values.
4. Separated input features and target variable.
5. Identified numerical and categorical features.
6. Applied median imputation to numerical features.
7. Applied most-frequent imputation to categorical features.
8. Applied One-Hot Encoding to categorical features.
9. Split the dataset into training and testing sets using an 80:20 ratio.

---

## Exploratory Data Analysis

The project includes analysis of:

- Sale price distribution
- Correlation between numerical features
- Overall Quality and Sale Price
- Above Ground Living Area and Sale Price
- Actual vs Predicted prices
- Prediction errors
- Feature importance

Some important features identified during the analysis include:

- Overall Quality (`OverallQual`)
- Above Ground Living Area (`GrLivArea`)
- Total Basement Area (`TotalBsmtSF`)
- First Floor Area (`1stFlrSF`)
- Garage-related features
- Year Built

---

## Model Performance

The models were evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

### Results

| Model | MAE | RMSE | R² Score |
|---|---:|---:|---:|
| Linear Regression | $20,485.66 | $31,327.80 | 0.8720 |
| Random Forest Regressor | $17,465.29 | $28,554.98 | 0.8937 |

The Random Forest Regressor achieved an R² score of **0.8937** on the held-out test set.

---

## Project Structure

```text
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


Setup and Installation
1. Clone or download the project

Download the project folder to your computer.

2. Create a virtual environment
python -m venv .venv
3. Activate the virtual environment

For Windows:

.venv\Scripts\activate
4. Install the required libraries
pip install -r requirements.txt
5. Open the Jupyter Notebook
jupyter notebook

Open:

notebooks/Rajraushan_House_Price_Prediction_IBM.ipynb
6. Run the notebook

Run the notebook cells sequentially or use Run All.

Model Saving

The trained Random Forest model is saved using Joblib:

models/house_price_prediction_model.pkl

The saved model was loaded again to verify that it can successfully generate predictions.

Key Findings
House prices show a right-skewed distribution.
Overall Quality has a strong relationship with Sale Price.
Above Ground Living Area is also an important factor in predicting house prices.
Random Forest Regressor achieved better test-set metrics than the Linear Regression baseline.
Feature importance analysis provides insight into the variables that contribute most to the model's predictions.
Limitations
The model was evaluated using a single held-out test split.
External real-world housing data was not used for validation.
House prices can also be affected by factors that are not represented in the dataset.
Future Improvements

Future improvements could include:

Hyperparameter tuning
Cross-validation
Advanced feature engineering
Testing additional regression algorithms
Deployment as a web application
Integration with a user-friendly prediction interface
Conclusion

This project demonstrates an end-to-end Machine Learning workflow for house price prediction, including data loading, exploratory data analysis, preprocessing, model training, evaluation, feature importance analysis, and model saving.

The Random Forest Regressor achieved an R² score of 0.8937 on the held-out test set and was saved as the final trained model.

Author
Rajraushan Kumar
BCA – Data Science & AI
Gopal Narayan Singh University

Internship
AICTE | IBM SkillsBuild Data Analytics with AI Internship 2026

Conducted by BharatCares in association with AICTE and IBM.
