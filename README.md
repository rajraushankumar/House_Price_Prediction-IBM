# 🏠 House Price Prediction Using Machine Learning

## 🎓 AICTE | IBM SkillsBuild Academic Internship – Data Analytics with AI

A machine learning project developed as part of the **AICTE | IBM SkillsBuild Academic Internship – Data Analytics with AI**, conducted by **BharatCares** in association with **AICTE and IBM**.

The project analyzes residential property data and builds machine learning models to predict house sale prices.

---

## 👨‍💻 Project Information

| Information | Details |
|---|---|
| **Name** | Rajraushan Kumar |
| **Program** | BCA – Data Science & AI |
| **University** | Gopal Narayan Singh University |
| **Project** | House Price Prediction Using Machine Learning |
| **Domain** | Data Analytics & Machine Learning |
| **Organization** | BharatCares |
| **Duration** | 17 August 2026 – 30 September 2026 |
| **Mode** | Virtual |

---

## 📌 Project Overview

The objective of this project is to develop a machine learning system capable of predicting residential house prices based on property characteristics.

### Machine Learning Workflow

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

Two regression algorithms were implemented:

Linear Regression
Random Forest Regressor
🎯 Objectives
Analyze the house price dataset.
Understand relationships between property features and sale prices.
Handle missing values.
Perform exploratory data analysis.
Prepare numerical and categorical features.
Train regression models.
Evaluate model performance.
Analyze feature importance.
Save and verify the trained model.
📊 Dataset

House Prices: Advanced Regression Techniques

Source: Kaggle – House Prices Dataset

The dataset contains residential property information and corresponding sale prices.

Dataset Information	Value
Records	1,460
Explanatory Features	80
Target Variable	SalePrice
Problem Type	Regression
🔍 Exploratory Data Analysis

The project includes the following analyses:

Sale price distribution
Correlation analysis
Overall quality vs sale price
Living area vs sale price
Actual vs predicted prices
Prediction error analysis
Feature importance
📈 Sale Price Distribution

🔥 Correlation Heatmap

🏠 Overall Quality vs Sale Price

📐 Living Area vs Sale Price

📉 Actual vs Predicted Prices

📊 Prediction Error Analysis

⭐ Feature Importance

🤖 Machine Learning
🔧 Data Preprocessing

A Scikit-learn preprocessing pipeline was used.

Numerical missing values → Median Imputation
Categorical missing values → Most Frequent Imputation
Categorical variables → One-Hot Encoding
ColumnTransformer and Pipeline → Consistent preprocessing
🧠 Models Used

1. Linear Regression

Used as the baseline regression model.

2. Random Forest Regressor

Used as the main tree-based regression model.

Configuration:

n_estimators = 300
random_state = 42
n_jobs = -1
📊 Model Performance

The models were evaluated using:

MAE – Mean Absolute Error
RMSE – Root Mean Squared Error
R² – Coefficient of Determination
Model	MAE	RMSE	R²
Linear Regression	$20,485.66	$31,327.80	0.8720
Random Forest Regressor	$17,465.29	$28,554.98	0.8937

The Random Forest Regressor achieved an R² score of 0.8937 on the project test set and was saved as the final model.

⭐ Feature Importance

The Random Forest model identified several important features, including:

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
💾 Model Saving

The trained Random Forest model was saved using Joblib.

models/
└── house_price_prediction_model.pkl

The saved model was successfully loaded and verified for prediction.

📁 Project Structure
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
│   └── House_Price_Prediction_Project_Report_Rajraushan_Kumar.docx
│
├── requirements.txt
└── README.md
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
1. Clone the Repository
git clone https://github.com/rajraushankumar/House_Price_Prediction_IBM.git
cd House_Price_Prediction_IBM
2. Create a Virtual Environment
python -m venv .venv
3. Activate the Environment

Windows:

.venv\Scripts\activate
4. Install Dependencies
pip install -r requirements.txt
5. Open the Jupyter Notebook
notebooks/Rajraushan_House_Price_Prediction_IBM.ipynb
6. Run the Notebook

Select the project's Python environment and run all cells from beginning to end.

🔎 Key Findings
Overall house quality has an important relationship with sale price.
Above-ground living area is an important feature for price prediction.
Both numerical and categorical features contribute to the prediction model.
Random Forest Regressor achieved an R² score of 0.8937 on the test set.
The trained model was successfully saved using Joblib.
The saved model was successfully loaded and verified.
OverallQual and GrLivArea were among the most influential features.
🚀 Future Improvements
Hyperparameter tuning
Cross-validation
Advanced feature engineering
Outlier treatment
Target variable transformation
Additional regression algorithms
Model deployment
Web-based prediction interface
Interactive prediction dashboard
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
🎓 Internship

AICTE | IBM SkillsBuild Academic Internship – Data Analytics with AI

Conducted by: BharatCares in association with AICTE and IBM
Duration: 17 August 2026 – 30 September 2026
Mode: Virtual

👤 Author

Rajraushan Kumar

BCA – Data Science & AI
Gopal Narayan Singh University

GitHub: @rajraushankumar

📌 Project Highlights
✨ End-to-end Machine Learning project
📊 Exploratory Data Analysis and visualization
🤖 Two regression models implemented
🌲 Random Forest with 300 estimators
📈 Model evaluation using MAE, RMSE and R²
⭐ Feature importance analysis
💾 Trained model saved using Joblib
📓 Complete Jupyter Notebook
📄 Complete project report
📋 Complete project documentation
⭐ Thank You

Thank you for visiting this project repository.

If you find this project useful, feel free to explore the notebook, visualizations, and project documentation.