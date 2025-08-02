# 🚗 Used Car Sales Prediction using Machine Learning

This project aims to build a predictive model that determines whether a used car will be sold based on various features such as brand, model, year, fuel type, kilometers driven, price, and seller type. The goal is to help car sellers and dealerships make better decisions by understanding the key factors influencing car sales.

## 📌 Problem Statement

> **Can we predict if a used car will be sold based on its attributes like price, brand, year, and usage?**

Predicting car sales helps sellers optimize inventory, set competitive prices, and target the right customers using data-driven strategies.

---

## 📊 Dataset Overview

- Total Records: ~200+
- Features:
  - `Brand`
  - `Model`
  - `Year`
  - `Fuel Type`
  - `Price`
  - `Kilometers Driven`
  - `Seller Type`
  - `Transmission`
  - `Engine Size`
  - `Sold` (Target: Yes / No)

---

## 🧪 Steps Performed

### 🔹 1. Data Preprocessing
- Handled missing values (mean imputation for numerical fields)
- Converted categorical features using One-Hot Encoding
- Applied logarithmic transformation to skewed data (`Kilometers Driven`)
- Created derived features:
  - `Car_Age`
  - `Price_per_year`
  - `KM_per_year`

### 🔹 2. Exploratory Data Analysis (EDA)
- Analyzed most frequently sold car brands
- Visualized price trends with kilometers driven
- Explored correlation patterns and distributions

### 🔹 3. Feature Engineering
- Generated new metrics (normalized values)
- Scaled numerical features using `StandardScaler`

### 🔹 4. Handling Class Imbalance
- Applied **SMOTE** (Synthetic Minority Over-sampling Technique) to oversample the minority class ('Sold')

### 🔹 5. Model Building
Tested multiple classification models:
- Logistic Regression
- Decision Tree
- Random Forest
- K-Nearest Neighbors (KNN)
- Gradient Boosting
- XGBoost

### 🔹 6. Hyperparameter Tuning
- Used `GridSearchCV` with `StratifiedKFold` and F1-score optimization

### 🔹 7. Ensemble Modeling
- Built a **Stacking Classifier** using top-performing models:
  - Base Models: Random Forest, Gradient Boosting, XGBoost
  - Final Estimator: Logistic Regression

---

## 📈 Evaluation Metrics

| Model              | Accuracy | F1-Score (Sold) | Precision (Sold) | Recall (Sold) |
|-------------------|----------|------------------|-------------------|---------------|
| Random Forest      | 0.68     | 0.64             | 0.55              | 0.80          |
| Logistic Regression| 0.53     | 0.62             | 0.55              | 0.70          |
| Gradient Boosting  | 0.70     | 0.65             | 0.60              | 0.72          |
| XGBoost            | 0.70     | 0.66             | 0.62              | 0.72          |
| **Stacking Classifier** | **0.60** | **0.71** | **0.56** | **1.00** |

📌 **Conclusion**: The Stacking Classifier achieved the best F1-score (0.71) and perfect recall (1.00) for the 'Sold' class, indicating excellent ability to identify actual sold cars.

---

## 📊 Visualizations

- Most Sold Car Brands (Bar Chart, Pie Chart)
- Price vs Kilometers Driven (Scatter Plot)
- Confusion Matrix (Stacking Classifier)
- Model Comparison Table

(*Visuals are available in the report/notebook.*)

---

## 🚀 Technologies Used

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- XGBoost
- Imbalanced-learn (SMOTE)
- Jupyter Notebook

---

## 📄 Report & Files

- 🔗 [Project Report PDF](./BIT%20Sindri%20Internship%20Report%201.pdf)
- 📓 [Jupyter Notebook](./Cars.ipynb)

---

## ✅ Future Improvements

- Incorporate features like `owner history`, `time on market`, or `location`
- Use advanced ensemble techniques like LightGBM or CatBoost
- Deploy the model using Flask or Streamlit for real-time predictions

---

## 🧑‍💻 Author

**Animesh Kumar Singh**  
B.Tech (CSE - IoT)  
Government Engineering College Vaishali  
📅 Internship at B.I.T Sindri | June–July 2025  
🔗 [GitHub Profile](https://github.com/animesh713331)

---

