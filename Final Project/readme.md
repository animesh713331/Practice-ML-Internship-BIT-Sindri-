# 🚗 Car Sales Prediction using Machine Learning

This project uses supervised machine learning to **predict whether a used car will be sold or not**, based on various features such as brand, model, year, fuel type, price, kilometers driven, and seller type. The goal is to assist car sellers or dealerships in making data-driven decisions about pricing, inventory, and marketing.

> 📍 Internship Project submitted to B.I.T Sindri (June–July 2025) under the guidance of Dr. Rajeev Ranjan and Mr. Vikash Kumar Singh.

---

## 🔍 Problem Statement

Predict whether a used car will be **sold or not sold** based on its features.

---

## 🧰 Technologies & Libraries Used

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-Learn
- XGBoost
- GridSearchCV

---

## 📊 Dataset Features

- `Brand`  
- `Model`  
- `Year`  
- `Fuel Type`  
- `Price`  
- `Kilometers Driven`  
- `Seller Type`  
- `Sold` (Target Variable)

---

## 🔬 Project Workflow

1. **Data Cleaning & Preprocessing**
   - Handled missing values
   - Converted categorical to numeric via One-Hot Encoding
   - Feature scaling and transformation

2. **Feature Engineering**
   - `Car_Age = 2025 - Year`
   - `Log_KM` (log transformation)
   - `Brand Frequency`

3. **EDA (Exploratory Data Analysis)**
   - Most sold brands (bar plot, pie chart)
   - Price vs. Kilometers driven (scatter plot)
   - Insights into trends affecting car sales

4. **Model Building**
   - Trained multiple classifiers:
     - Logistic Regression
     - Decision Tree
     - Random Forest ✅ (Best Model)
     - KNN
     - Gradient Boosting
     - XGBoost
   - Hyperparameter tuning using GridSearchCV

5. **Model Evaluation**
   - Accuracy, Precision, Recall, F1-Score
   - Confusion Matrix

---

## 🏆 Best Model Performance: Random Forest

| Metric        | Score |
|---------------|-------|
| Accuracy      | 0.60  |
| Precision     | 0.63  |
| Recall        | 0.57  |
| F1-Score      | 0.60  |

---

## 📌 Key Insights

- **Honda, Kia, Ford, and Maruti** were the top-selling car brands.
- Cars with **lower kilometers driven and lower age** are more likely to sell.
- Random Forest showed the best balance of performance metrics for binary classification.

---

## 📈 Future Improvements

- Use more advanced models like **LightGBM or CatBoost**.
- Apply **SMOTE** to balance the target classes.
- Deploy the model using **Streamlit** or **Flask**.
- Add **feature importance visualization** using SHAP or permutation methods.

---

## 📝 Report

The complete internship report (`BIT Sindri Internship Report.pdf`) contains:
- Abstract
- Full analysis & visuals
- Results
- Model evaluation
- Conclusion

---

## 👨‍💻 Author

**Animesh Kumar Singh**  
- B.Tech, Computer Science & Engineering (IoT), Government Engineering College Vaishali  
- Internship at B.I.T Sindri, under Prof. Vikash Kumar Singh & Dr. Rajeev Ranjan  
- 📅 Internship Duration: *June 5 – July 11, 2025*

---

## 📜 License

This project is part of an academic internship submission. Free to use for learning and non-commercial purposes. Attribution appreciated.

