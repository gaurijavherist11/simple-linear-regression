📘 Simple Linear Regression – Salary Prediction Project

This project demonstrates how to build a Simple Linear Regression model to predict Salary based on Years of Experience using Python, Scikit-Learn, and Statsmodels.

The project includes dataset loading, preprocessing, model building, evaluation, and individual prediction.
Both Jupyter Notebook (.ipynb) and an exported HTML version are included for easy viewing.

📁 Project Structure
📦 Simple Linear Regression Project
│
├── README.md                                   # Project documentation
├── Salary_dataset.csv                           # Dataset used for regression
├── Simple linear regression practical.ipynb      # Main Jupyter Notebook
└── Simple linear regression practical (3).html   # Exported notebook for easy viewing

🚀 Project Overview

This project covers the complete workflow of building and evaluating a simple linear regression model, including:

✔ Data Loading & Exploration

Importing the Salary dataset

Inspecting features and target variable

Visualizing data with scatter plots

✔ Train–Test Split

Splitting dataset into training and testing sets for model evaluation.

✔ Feature Scaling

Using StandardScaler to scale:

Input feature (Years of Experience)

Target variable (Salary)

This helps the regression model train more efficiently.

✔ Model Building
1️⃣ Scikit-Learn LinearRegression

Training regression model

Extracting slope (coefficient) and intercept

Making predictions

Predicting salary for individual values

2️⃣ Statsmodels OLS Regression

Building Ordinary Least Squares model

Generating detailed model summary (coef, p-values, R², etc.)

Comparing coefficients with sklearn model

📊 Model Evaluation

The model is evaluated using the following metrics:

Mean Squared Error (MSE)

Mean Absolute Error (MAE)

Root Mean Squared Error (RMSE)

Evaluation is shown using:

Original salary values

Scaled values

🔍 Individual Prediction

The project includes an example of predicting salary for a given experience value.

# Predicting salary for new experience value
regression.predict(scaler_X.transform([[12]]))


If the target is scaled, predictions are converted back to original salary using inverse transform.

🛠 Technologies Used

Python

Jupyter Notebook

NumPy

Pandas

Scikit-Learn

Statsmodels

Matplotlib

📌 Future Enhancements

Add Polynomial Regression

Add Multiple Linear Regression

Build a Streamlit or Flask Web App for deployment

Add model interpretation (Residuals, QQ-plot, etc.)

🙌 Acknowledgments

This project was built to practice Machine Learning fundamentals:

Data preprocessing

Scaling

Linear regression

Model interpretation

Evaluation metrics

The data set which i used is from https://www.kaggle.com/datasets/karthickveerakumar/salary-data-simple-linear-regression
