# 🏅 Olympic Athletes Data Cleaning & Analysis

A complete data analysis project focused on cleaning, exploring, and interpreting the *Olympic Athletes Events Dataset*.  
This project aims to understand athlete characteristics, identify meaningful patterns, and prepare the dataset for potential advanced modeling.

---

## 📌 Project Overview

This project illustrates a full **data cleaning and exploratory data analysis (EDA) workflow**.  
It includes:

- 🧹 Data Cleaning & Preprocessing  
- 📊 Exploratory Data Analysis (EDA)  
- 🧮 Feature Engineering (IMC/BMI, quantiles…)  
- 📦 Outlier Detection & Treatment  
- 📈 Statistical Visualization  
- 📝 Interpretations and insights

**Dataset Source:**  
[Kaggle – 120 Years of Olympic Athletes and Results](https://www.kaggle.com/datasets/abdullahmeo/120-years-of-olympic-athletes-dataset)

---

## 📁 Dataset Description

This dataset contains detailed information about Olympic athletes between 1896 and 2016.

| Feature | Description |
|--------|-------------|
| **ID** | Athlete identifier |
| **Name** | Athlete name |
| **Sex** | M / F |
| **Age** | Athlete age |
| **Height** | Height (cm) |
| **Weight** | Weight (kg) |
| **NOC** | Country code |
| **Year** | Olympic year |
| **Season** | Summer / Winter |
| **City** | Host city |
| **Sport** | Sport category |
| **Event** | Specific event |
| **Medal** | Gold / Silver / Bronze / No medal |

---

## 🧹 Data Cleaning & Preprocessing

### ✔ 1. Duplicate Removal
- Removed exact duplicate rows to ensure dataset consistency.

### ✔ 2. Handling Missing Values
- Filled missing Age, Height, and Weight using **median imputation**.
- Replaced missing medals with `"No medal"`.

### ✔ 3. Feature Engineering
A new feature was created:

\[
IMC = \frac{Poids}{(Taille/100)^2}
\]

This helps analyze athletes’ physical profiles beyond raw height/weight.

### ✔ 4. Outlier Detection & Removal
- Used **IQR (Interquartile Range)** method to detect and remove extreme values.
- Cleaned IMC distribution for better visual analysis.

### ✔ 5. Data Organization
- Deleted irrelevant columns (Games, Team).
- Reordered variables for readability.
- Inserted IMC at column index 4.

---

## 📊 Exploratory Data Analysis (EDA)

The EDA includes:

### 🔹 Age Distribution
- Kernel Density Estimation (KDE) to identify the typical age of Olympic athletes.
- Most athletes are between **20–30 years**.

### 🔹 IMC (BMI) Distribution
- Boxplots before and after cleaning.
- Majority of IMC values fall between **21–24**.
- Outliers detected and removed using IQR.

### 🔹 Medal Distribution by Sex
- Male athletes account for ~70% of medals.
- Reflects historical imbalance in Olympic participation.

### 🔹 Top Countries by Medal Count
- Ranking based on NOC.
- Visualized using bar charts.

---

## 📈 Visualizations Included

- KDE plots (Age, IMC)
- Boxplots (IMC overall, IMC by Medal)
- Bar charts (Medals by Sex, Medals by Country)
- Quantile tables & statistical summaries

All plots are accompanied by interpretations.

---

## 🧠 Key Insights

- Peak athletic performance age is around **20–25 years**.
- IMC is relatively stable among athletes, clustering around **22–24**.
- Outliers in IMC are often tied to specific sports or data inconsistencies.
- Male athletes historically dominate Olympic medal counts.
- Certain nations consistently rank among top performers.

---

## 📦 Project Structure
Olympic-Athletes-Analysis/
├── Olympic Athletes Data Cleaning And Analysis.ipynb
├── Olympic Athletes Data Cleaning And Analysis.html
└── README.md
---

## 🚀 Future Work

Potential future extensions:

- Analyze trends by Olympic era  
- Compare Summer vs Winter athletes  
- Cluster athletes by physical metrics (Age, IMC, Sport…)  
- Build predictive models:
  - Medal prediction  
  - Sport classification  
  - Athlete profiling  

---

## ✨ Author

**Maghraoui Nour**  
Big Data & Data Analysis Student  
