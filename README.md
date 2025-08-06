# 🧹 Titanic Dataset - Data Cleaning & Preprocessing

## 📌 Objective
This project focuses on cleaning and preprocessing raw data from the Titanic dataset in preparation for machine learning models.

---

## 🛠 Tools & Libraries Used
- Python
- Pandas
- NumPy
- Seaborn & Matplotlib
- scikit-learn

---

## 📊 Dataset Info
- **Dataset**: Titanic survival dataset (from Kaggle)
- **Rows**: 891
- **Columns**: 12 (including numeric and categorical)

---

## 🔍 Steps Performed

### 1. Data Exploration
- Viewed shape, data types, and summary stats
- Checked missing values using `.isnull().sum()`

### 2. Handling Missing Values
- Filled missing `Age` with median
- Filled missing `Embarked` with mode
- Dropped `Cabin` (more than 77% missing)

### 3. Encoding Categorical Features
- Label encoded `Sex` (male = 0, female = 1)
- One-hot encoded `Embarked` and dropped the first category to avoid dummy variable trap

### 4. Feature Scaling
- Applied `StandardScaler` to normalize `Age` and `Fare`

### 5. Outlier Detection & Removal
- Used boxplots to visualize outliers
- Removed Fare outliers above the 99th percentile

---

## ✅ Output
- Cleaned, numeric dataset ready for ML modeling
- Final shape: (881, 11)
- No missing values
- Scaled and encoded features

---


