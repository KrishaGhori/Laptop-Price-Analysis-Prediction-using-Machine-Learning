# Laptop-Price-Analysis-Prediction-using-Machine-Learning

A complete end-to-end data science project that predicts laptop prices based on various specifications using **Python** and **Scikit-learn**. The project includes data cleaning, exploratory data analysis (EDA), feature preprocessing with pipelines, and model comparison.

![Actual vs Predicted](images/actual_vs_predicted.png)  

---

## 📋 Project Overview

This project analyzes a dataset of 1,275 laptops and builds machine learning models to predict their prices in euros. After comparing multiple models, **Random Forest Regressor** was selected as the best-performing model.

### Key Highlights:
- Cleaned and preprocessed real-world laptop data
- Built a robust preprocessing pipeline (numerical + categorical features)
- Trained and evaluated 3 models: Linear Regression, Decision Tree, and Random Forest
- Random Forest achieved the lowest RMSE and best generalization

---

## 🛠️ Technologies Used

- **Python**
- Pandas, NumPy
- Matplotlib & Seaborn (Visualization)
- Scikit-learn (Modeling & Pipelines)
- Jupyter Notebook

---

## 📁 Dataset

- **Source**: `laptop_prices.csv`
- **Target Variable**: `Price_euros`
- **Features**:
  - Company, Product, TypeName
  - Inches, Ram, Weight
  - Screen resolution, Touchscreen, IPS Panel, Retina Display
  - CPU (company, frequency, model)
  - Storage (Primary & Secondary, type)
  - GPU (company & model)
  - OS

---

## 📊 Project Workflow

1. **Data Loading & Exploration**
2. **Data Cleaning** (Null values, duplicates)
3. **Exploratory Data Analysis**
4. **Feature Engineering** using `ColumnTransformer` + `Pipeline`
5. **Model Training & Evaluation**
   - Linear Regression
   - Decision Tree Regressor
   - Random Forest Regressor
6. **Model Comparison** using Cross-Validation (RMSE)
7. **Final Model**: Random Forest Regressor
8. **Prediction & Visualization**

---

## 📈 Results

| Model                | Training RMSE | CV Mean RMSE     | Remarks                  |
|----------------------|---------------|------------------|--------------------------|
| Linear Regression    | 97.12         | 333.60           | Underfits                |
| Decision Tree        | 16.45         | 365.58           | Overfits                 |
| **Random Forest**    | **102.25**    | **275.61**       | **Best Model**           |

**Conclusion**: Random Forest provided the best balance between accuracy and generalization.
