# 📈 Multiple Linear Regression – Economic Dataset

This project demonstrates **Multiple Linear Regression** using an economics-based dataset to understand relationships between macroeconomic factors and an index price. The notebook focuses on **data understanding, visualization, model building, and diagnostic analysis using residuals**.

---

## 📌 Project Objective

To analyze how economic indicators such as **interest rate** and **unemployment rate** influence the **index price**, and to validate a multiple linear regression model using proper statistical assumptions.

---

## 🗂️ Dataset Description

The dataset contains the following variables:

| Column Name         | Description                   |
| ------------------- | ----------------------------- |
| `interest_rate`     | Interest rate (%)             |
| `unemployment_rate` | Unemployment rate (%)         |
| `index_price`       | Economic / market index price |

---

## 🧪 Techniques & Methods Used

### 1️⃣ Exploratory Data Analysis (EDA)

* Scatter plots to understand relationships between:

  * Interest rate vs Index price
  * Unemployment rate vs Index price
* Pair plots to visualize multivariate relationships
* Correlation matrix to quantify strength and direction of relationships

**Purpose:** Identify trends, direction (positive/negative), and suitability for regression.

---

### 2️⃣ Correlation Analysis

* Used Pearson correlation coefficient
* Findings:

  * Strong positive correlation between `interest_rate` and `index_price`
  * Weak inverse (negative) correlation between `unemployment_rate` and `index_price`

**Note:** Both positive and negative correlations are valid for multiple linear regression.

---

### 3️⃣ Data Visualization Techniques

Libraries used:

* `matplotlib`
* `seaborn`

Plots created:

* `plt.scatter()` for feature vs target visualization
* `sns.regplot()` to visualize regression line with data points
* `sns.displot(kind='kde')` for residual distribution

---

### 4️⃣ Model Building – Multiple Linear Regression

* Independent variables (X):

  * Interest rate
  * Unemployment rate
* Dependent variable (Y):

  * Index price

The model learns a linear relationship of the form:

> **Index Price = β₀ + β₁(Interest Rate) + β₂(Unemployment Rate)**

---

### 5️⃣ Model Diagnostics – Residual Analysis

Residuals were analyzed to validate regression assumptions:

#### ✔ Residuals without drift

* Randomly scattered around zero
* Indicates unbiased predictions

#### ✔ Normality of residuals

* Residuals approximately follow a bell-shaped (normal) distribution
* Checked using KDE plot

#### ✔ Interpretation

* Slight skewness is acceptable in real-world data
* Residuals centered near zero indicate a good model fit

---

## 📊 Key Statistical Concepts Applied

* Uniform vs Normal vs Regression data
* Correlation vs causation
* Positive vs negative correlation
* Residuals:

  * Residuals near zero
  * Mean of residuals ≈ 0
  * Random distribution above and below zero
* Difference between:

  * Residuals with drift vs without drift
  * Raw data distribution vs residual distribution

---

## 🛠️ Libraries Used

```python
numpy
pandas
matplotlib
seaborn
scikit-learn
```

---

## ✅ Conclusion

* The data is **not uniformly distributed**, which is expected and desirable for regression
* The regression model successfully captures the linear relationship
* Residual diagnostics confirm the model is statistically acceptable
* The project demonstrates a complete end-to-end regression workflow

---

## 📌 Author

**Gauri Milind Javheri**
(Data Science / ML Learner)

---

## 📘 Learning Outcome

This project strengthens understanding of:

* Multiple Linear Regression
* Economic data analysis
* Residual-based model validation
* Practical ML reasoning beyond just accuracy

