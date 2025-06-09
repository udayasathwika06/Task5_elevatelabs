# Task5_elevatelabs
# 🚢 Titanic Dataset - Exploratory Data Analysis (EDA)

This repository contains an Exploratory Data Analysis (EDA) of the Titanic dataset as part of **ElevateLabs Task 5**.

## 📁 Files Included

- `train.csv` – The original Titanic dataset used for analysis.
- `Task5_report.pdf` – PDF version of the final EDA summary.
- `task5.ipynb` – Python script performing step-by-step EDA using Pandas, Seaborn, and Matplotlib.

---

## 📊 Objective

The goal of this task is to explore the Titanic dataset to understand the patterns behind passenger survival using descriptive statistics and visualizations.

---

## 🧰 Libraries Used

- `pandas` – For data manipulation.
- `matplotlib.pyplot` – For basic plotting.
- `seaborn` – For enhanced statistical visualizations.

---

## 🔍 EDA Process

### 1. Dataset Overview

- **Total passengers**: 891
- Key features: `Survived`, `Pclass`, `Sex`, `Age`, `SibSp`, `Parch`, `Fare`, `Embarked`
- **Missing Values**:
  - `Age`: ~19.8% missing
  - `Cabin`: ~77% missing
  - `Embarked`: 2 missing entries

### 2. Univariate Analysis

- **Histograms** for `Age` and `Fare`:
  - Age is bell-shaped, most passengers were aged 20–40.
  - Fare is right-skewed; most passengers paid lower fares.

- **Count Plots**:
  - More passengers died than survived.
  - Most were in 3rd class (lowest).

### 3. Bivariate Analysis

- **Boxplots**:
  - 1st class passengers were older and paid significantly more.
  - Fare outliers are notable, especially in 1st class.

- **Correlation Heatmap**:
  - `Survived` is negatively correlated with `Pclass` and positively with `Fare`.

- **Pairplot**:
  - Survivors tend to cluster in high fare and lower Pclass zones.

---

## 📌 Key Insights

- Majority of passengers were in 3rd class, and most of them didn’t survive.
- Survival rates were higher for 1st class passengers.
- Fare and class are strong indicators of survival chances.
- Age and Fare distributions are skewed; imputation and transformations may be necessary.
- Although not visualized here, **gender** also plays a major role—females had higher survival rates.

---

## ✅ Next Steps (for ML modeling)

- Handle missing data (e.g., impute `Age`, drop or engineer around `Cabin`).
- Encode categorical variables (`Sex`, `Embarked`).
- Engineer features like `FamilySize`, `Title` (from `Name`).
- Scale/transform skewed features (`Fare`).

---


