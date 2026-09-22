# 🏠 House Price Prediction Using Machine Learning

## 🎓 AICTE | IBM SkillsBuild Academic Internship – Data Analytics with AI

Welcome to my **House Price Prediction** machine learning project.

This project was developed as part of the **AICTE | IBM SkillsBuild Academic Internship – Data Analytics with AI**, conducted by **BharatCares** in association with **AICTE and IBM**.

The project focuses on analyzing residential property data and building machine learning models to predict house sale prices.

---

## 👨‍💻 Project Information

- **Name:** Rajraushan Kumar
- **Program:** BCA – Data Science & AI
- **University:** Gopal Narayan Singh University
- **Project:** House Price Prediction Using Machine Learning
- **Internship:** AICTE | IBM SkillsBuild Academic Internship
- **Domain:** Data Analytics & Machine Learning
- **Organization:** BharatCares
- **Internship Duration:** 17 August 2026 – 30 September 2026
- **Mode:** Virtual

---

## 📌 Project Overview

The objective of this project is to develop a machine learning system capable of predicting residential house prices based on various property characteristics.

The project follows a complete machine learning workflow:

```text
Data Collection
      ↓
Data Understanding
      ↓
Data Cleaning
      ↓
Exploratory Data Analysis
      ↓
Data Preprocessing
      ↓
Model Training
      ↓
Model Evaluation
      ↓
Feature Importance Analysis
      ↓
Model Saving

Two regression algorithms were implemented and evaluated:

Linear Regression
Random Forest Regressor


🎯 Objectives

The main objectives of this project are:

Analyze the house price dataset.
Understand relationships between property features and sale prices.
Identify important features affecting house prices.
Handle missing values.
Perform exploratory data analysis.
Prepare numerical and categorical data for machine learning.
Train regression models.
Evaluate model performance.
Analyze feature importance.
Save and verify the trained machine learning model.
📊 Dataset
House Prices: Advanced Regression Techniques

Source: Kaggle

The dataset contains information about residential properties and their corresponding sale prices.

Dataset Details
Information	Value
Records	1,460
Explanatory Features	80
Target Variable	SalePrice
Problem Type	Regression
Target Variable
SalePrice

The model uses the available property features to predict the final sale price of a house.

🔍 Exploratory Data Analysis

Exploratory Data Analysis was performed to understand the distribution of house prices and relationships between important features.

The analysis includes:

Sale price distribution
Correlation analysis
Overall quality vs sale price
Living area vs sale price
Actual vs predicted prices
Prediction error analysis
Feature importance
📈 Sale Price Distribution

This visualization shows the distribution of residential property sale prices.

🔥 Correlation Heatmap

The correlation heatmap helps identify relationships between numerical variables in the dataset.

🏠 Overall Quality vs Sale Price

This visualization shows the relationship between the overall quality of a property and its sale price.

📐 Living Area vs Sale Price

This visualization shows the relationship between above-ground living area and house sale price.

📉 Actual vs Predicted Prices

This visualization compares the actual house prices from the test dataset with the prices predicted by the Random Forest model.

📊 Prediction Error Analysis

The prediction error distribution was analyzed to understand how the model's predictions differ from the actual house prices.

⭐ Feature Importance

Feature importance analysis was performed using the trained Random Forest model.

The analysis identified important features contributing to the model's predictions.

Important features included:

OverallQual
GrLivArea
TotalBsmtSF
2ndFlrSF
BsmtFinSF1
1stFlrSF
LotArea
GarageArea
GarageCars
YearBuilt
🤖 Machine Learning
🔧 Data Preprocessing

A Scikit-learn preprocessing pipeline was used to prepare the data.

Numerical Features

Missing numerical values were handled using median imputation.

Categorical Features

Missing categorical values were handled using most frequent value imputation.

Categorical variables were converted into numerical representations using One-Hot Encoding.

A ColumnTransformer and Pipeline were used to maintain a consistent preprocessing workflow.

🧠 Models Used
1. Linear Regression

Linear Regression was implemented as a baseline regression model.

2. Random Forest Regressor

Random Forest Regressor was implemented as the main tree-based regression model.

Configuration
n_estimators = 300
random_state = 42
n_jobs = -1
📊 Model Performance

The models were evaluated using three standard regression metrics:

MAE – Mean Absolute Error
RMSE – Root Mean Squared Error
R² – Coefficient of Determination
Model	MAE	RMSE	R²
Linear Regression	$20,485.66	$31,327.80	0.8720
Random Forest Regressor	$17,465.29	$28,554.98	0.8937

The Random Forest Regressor achieved an R² score of 0.8937 on the project's test set and was saved as the final model.

💾 Model Saving

The trained Random Forest model was saved using Joblib.

models/
└── house_price_prediction_model.pkl

The saved model was subsequently loaded and successfully verified for prediction.

##📁 **Project Structure**
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
│   ├── feature_importance.png
│   ├── House_Price_Prediction_Project_Report_Rajraushan_Kumar.docx
│   └── House_Price_Prediction_Project_Report_Rajraushan_Kumar.pdf
│
├── requirements.txt
└── README.md

The .venv virtual environment is used locally for development and is not required for the final project submission.

🛠️ Technologies Used
🐍 Python
🐼 Pandas
🔢 NumPy
📊 Matplotlib
📈 Seaborn
🤖 Scikit-learn
📓 Jupyter Notebook
💾 Joblib
📗 OpenPyXL
▶️ How to Run the Project
Step 1 – Open the Project

Open the House_Price_Prediction_IBM folder in VS Code.

Step 2 – Create a Virtual Environment
python -m venv .venv
Step 3 – Activate the Virtual Environment

For Windows:

.venv\Scripts\activate
Step 4 – Install Required Libraries
pip install -r requirements.txt
Step 5 – Open the Jupyter Notebook

Open:

notebooks/Rajraushan_House_Price_Prediction_IBM.ipynb
Step 6 – Select the Python Kernel

Select the Python interpreter from the project's .venv environment.

Step 7 – Run the Notebook

Run all cells from beginning to end.

🔎 Key Findings

The project produced the following observations:

Overall house quality has an important relationship with sale price.
Above-ground living area is an important feature for price prediction.
Numerical and categorical features both contribute to the prediction model.
Random Forest Regressor achieved an R² score of 0.8937 on the test set.
The trained model was successfully saved using Joblib.
The saved model was successfully loaded and verified.
Feature importance analysis identified OverallQual and GrLivArea among the most influential features.
🚀 Future Improvements

The project can be further improved through:

Hyperparameter tuning
Cross-validation
Advanced feature engineering
Outlier treatment
Target variable transformation
Additional regression algorithms
Model deployment
Web-based prediction interface
Interactive house price prediction dashboard
📚 Project Learning Outcomes

Through this project, I gained practical experience in:

Data cleaning
Exploratory data analysis
Data visualization
Numerical and categorical preprocessing
Machine learning pipelines
Regression algorithms
Model evaluation
Feature importance analysis
Model persistence using Joblib
Project documentation
GitHub project organization

## 🎓 **Internship**

This project was completed as part of:

AICTE | IBM SkillsBuild Academic Internship – Data Analytics with AI

Conducted by: BharatCares in association with AICTE and IBM

Duration: 17 August 2026 – 30 September 2026

Mode: Virtual


## 👤 **Author**
Rajraushan Kumar

BCA – Data Science & AI
Gopal Narayan Singh University

GitHub: @rajraushankumar

📌 Project Highlights

✨ End-to-end machine learning project

📊 Exploratory data analysis and visualization

🤖 Two regression models implemented

🌲 Random Forest with 300 estimators

📈 Model evaluation using MAE, RMSE and R²

⭐ Feature importance analysis

💾 Trained model saved using Joblib

📓 Complete Jupyter Notebook

📄 Complete project report

📋 Complete project documentation

# ⭐ **Thank You**
Thank you for visiting this project repository.

If you find this project useful, feel free to explore the notebook, visualizations, and project documentation.
