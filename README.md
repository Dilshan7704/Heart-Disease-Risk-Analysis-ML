# ❤️ Heart Disease Risk Analysis ML

<div align="center">

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange?style=for-the-badge&logo=scikitlearn)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-black?style=for-the-badge&logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-blue?style=for-the-badge&logo=numpy)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Project-Completed-success?style=for-the-badge)

### 🫀 Machine Learning Project for Heart Disease Risk Prediction

Predicting heart disease risk using Machine Learning, PCA, EDA, Data Visualization, and advanced Classification Algorithms.

</div>

---

# 📌 Project Overview

Heart disease is one of the leading causes of death worldwide.  
This project focuses on building a complete Machine Learning pipeline capable of predicting heart disease risk accurately using patient medical attributes.

The project includes:

✔ Data Cleaning & Preprocessing  
✔ Exploratory Data Analysis (EDA)  
✔ Data Visualization  
✔ PCA Dimensionality Reduction  
✔ Model Training & Comparison  
✔ Hyperparameter Tuning  
✔ Threshold Optimization  
✔ Model Evaluation  
✔ Risk Prediction System  
✔ Model Serialization using Joblib  

---

# 🗂️ Project Structure

```bash
HEART-DISEASE-RISK-ANALYSIS-ML/
│
├── 📁 Data set/
│   └── heart_desease.csv
│
├── 📁 Models/
│   │
│   ├── 📁 with_out_pca_models/
│   │   ├── CatBoost_model.pkl
│   │   ├── RandomForest_model.pkl
│   │   ├── Logistic_model.pkl
│   │   └── ...
│   │
│   ├── 📁 With_pca_models/
│   │   ├── CatBoost_pca_model.pkl
│   │   ├── RandomForest_pca_model.pkl
│   │   └── ...
│   │
│   ├── final_heart_disease_model.pkl
│   ├── pca_model.pkl
│   ├── x_train.pkl
│   ├── x_test.pkl
│   ├── y_train.pkl
│   ├── y_test.pkl
│   ├── x_train_pca.pkl
│   └── x_test_pca.pkl
│
├── 📁 src/
│   ├── data_preprocessing.ipynb
│   ├── model_training.ipynb
│   ├── evaluation.ipynb
│   └── prediction.ipynb
│
├── 📄 requirements.txt
├── 📄 .gitignore
└── 📄 README.md
```

---

# ⚙️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Programming Language |
| Pandas | Data Manipulation |
| NumPy | Numerical Operations |
| Matplotlib | Data Visualization |
| Seaborn | Statistical Visualization |
| Scikit-learn | Machine Learning |
| CatBoost | Gradient Boosting |
| LightGBM | Gradient Boosting |
| Joblib | Model Serialization |

---

# 📊 Exploratory Data Analysis (EDA)

Extensive Exploratory Data Analysis was performed to understand patterns and relationships between patient health indicators and heart disease risk.

### 🔍 EDA Includes

- Missing Value Analysis
- Duplicate Detection
- Target Variable Distribution
- KDE Distribution Plots
- Histogram Analysis
- Boxplot Visualization
- Correlation Heatmaps
- Feature Correlation with Target
- Outlier Detection & Cleaning

---

# 📈 Visualizations

The project includes multiple visualizations such as:

✅ Heart Disease Distribution  
✅ KDE Distribution by Target Class  
✅ Histogram Distributions  
✅ Boxplots for Outlier Detection  
✅ Correlation Heatmaps  
✅ Model Comparison Charts  
✅ Confusion Matrix  
✅ ROC Curve Analysis  

---

# ⚠️ Data Preprocessing

Data preprocessing steps performed:

- Handling missing values
- Removing invalid cholesterol values
- Removing unrealistic age values
- Feature Scaling using StandardScaler
- PCA for dimensionality reduction
- Train-Test Splitting
- Saving processed datasets using Joblib

---

# 🧠 PCA Dimensionality Reduction

Principal Component Analysis (PCA) was implemented to reduce feature dimensions while preserving important information.

### PCA Benefits

✔ Reduced feature complexity  
✔ Faster model training  
✔ Reduced overfitting  
✔ Improved generalization  

The project compares:

- Models trained with PCA
- Models trained without PCA

---

# 🤖 Machine Learning Models

The following classification models were trained and evaluated:

| Model | Status |
|---|---|
| Logistic Regression | ✅ Tested |
| Support Vector Machine (SVM) | ✅ Tested |
| Decision Tree Classifier | ✅ Tested |
| Random Forest Classifier | ✅ Tested |
| LightGBM Classifier | ✅ Tested |
| CatBoost Classifier | ✅ Best Performance |
| Gaussian Naive Bayes | ✅ Tested |

---

# 🏆 Best Performing Model

## ✅ CatBoost Classifier

The CatBoost model achieved the best overall performance.

### Techniques Used

- Stratified K-Fold Cross Validation
- GridSearchCV Hyperparameter Tuning
- Threshold Optimization
- PCA Comparison
- F1 Score Optimization

---

# 📌 Evaluation Metrics

The models were evaluated using:

- Accuracy Score
- Precision
- Recall
- F1 Score
- Confusion Matrix
- ROC Curve
- AUC Score
- Classification Report

---

# 💾 Model Serialization

The trained models were saved using Joblib for future predictions.

```python
joblib.dump(model, "CatBoost_model.pkl")
```

---

# 🔮 Heart Disease Prediction System

A custom prediction system was implemented to classify patient heart disease risk.

### Prediction Output

- 🟢 Low Risk of Heart Disease
- 🔴 High Risk of Heart Disease

```python
prediction = model.predict(input_df)
```

---

# 📷 Sample Prediction Workflow

```text
Patient Medical Data
          ↓
Data Cleaning
          ↓
Feature Scaling
          ↓
PCA Transformation
          ↓
Model Prediction
          ↓
Risk Probability
          ↓
Final Heart Disease Risk Result
```

---

# ▶️ Installation & Usage

## 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/HEART-DISEASE-RISK-ANALYSIS-ML.git
```

---

## 2️⃣ Navigate to Project

```bash
cd HEART-DISEASE-RISK-ANALYSIS-ML
```

---

## 3️⃣ Install Required Libraries

```bash
pip install -r requirements.txt
```

---

## 4️⃣ Run Jupyter Notebook

```bash
jupyter notebook
```

Open:

```bash
src/data_preprocessing.ipynb
```

---

# 📚 Dataset Information

Dataset used for this project:

🔗 https://www.kaggle.com/

## Dataset Features

- Age
- Sex
- Chest Pain Type
- Blood Pressure
- Cholesterol
- FBS Over 120
- EKG Results
- Max Heart Rate
- Exercise Angina
- ST Depression
- Slope of ST
- Number of Vessels Fluoro
- Thallium

## Target Variable

| Value | Meaning |
|---|---|
| 0 | No Heart Disease |
| 1 | Heart Disease Present |

---

# 🚀 Future Improvements

Planned future enhancements:

- 🌐 Flask/FastAPI Deployment
- 📊 Streamlit Dashboard
- ⚡ Real-Time Prediction API
- ☁ Cloud Deployment
- 📱 Mobile-Friendly Frontend
- 🧠 Deep Learning Models
- 📈 Explainable AI (SHAP/LIME)

---

# 👨‍💻 Author

## Dilshan Nethmin Wijayarathne

💡 Machine Learning Enthusiast  
💻 Full Stack Developer  
📊 Data Analytics & AI Projects  

---

# ⭐ Support

If you found this project useful:

⭐ Star the repository  
🍴 Fork the project  
🛠️ Contribute to improvements  

---

<div align="center">

## ❤️ Thanks for Visiting

### 🫀 Heart Disease Risk Analysis using Machine Learning

</div>
