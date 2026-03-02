🏅 Olympic Medal Prediction
Data Cleaning • Exploratory Data Analysis • Machine Learning
<p align="center">
📌 Project Overview

This project focuses on:

✔ Data Cleaning & Preprocessing
✔ Exploratory Data Analysis (EDA)
✔ Feature Engineering
✔ Machine Learning Classification

The objective is to predict whether an athlete will win a medal or not based on demographic and competition features.

Dataset source:
🔗 Kaggle – Olympic Athlete Events Dataset

📂 Dataset Description

The dataset contains historical data about Olympic athletes, including:

Feature	Description
Age	Athlete age
Sex	Male / Female
Height	Height (cm)
Weight	Weight (kg)
Sport	Sport category
NOC	Country code
Year	Olympic year
Medal	Gold / Silver / Bronze / No medal
🧹 Data Cleaning & Preparation
🔹 1. Removing Duplicates

Checked duplicate rows across all columns

Dropped duplicates

🔹 2. Handling Missing Values

Replaced missing Height and Weight with median

Replaced missing Medal with "No medal"

🔹 3. Feature Engineering

Created a new feature:

📌 BMI (IMC)
𝐵
𝑀
𝐼
=
𝑊
𝑒
𝑖
𝑔
ℎ
𝑡
(
𝐻
𝑒
𝑖
𝑔
ℎ
𝑡
/
100
)
2
BMI=
(Height/100)
2
Weight
	​


Then removed Height and Weight to reduce redundancy.

🔹 4. Dropped Unnecessary Columns

Games

Team

🔹 5. Sorting & Resetting Index

Sorted by Age and Year.

📊 Exploratory Data Analysis
📈 1️⃣ Medal Percentage by Sex

Bar chart showing medal distribution between male and female athletes.

📈 2️⃣ BMI Distribution by Medal Type

Boxplot comparing BMI across:

🥇 Gold

🥈 Silver

🥉 Bronze

📈 3️⃣ Top 20 Countries by Medal Count

Grouped by NOC.

🤖 Machine Learning Model
🎯 Target Variable
df['HasMedal'] = (df['Medal'].isin(['Gold','Silver','Bronze'])).astype(int)

1 → Won a medal

0 → No medal

🧠 Model Used

✔ Logistic Regression
✔ OneHot Encoding for categorical features
✔ Train/Test Split (80/20)
✔ Scikit-Learn Pipeline

Features Used:

Age

BMI

Sex

Sport

NOC

📊 Model Performance
print("Accuracy :", model.score(X_test, y_test))

The model outputs an accuracy score representing prediction performance.

🛠 Tech Stack
Tool	Purpose
Python	Programming
Pandas	Data manipulation
NumPy	Numerical operations
Matplotlib	Visualization
Seaborn	Statistical plots
Scikit-learn	Machine Learning
📁 Project Structure
📦 Olympic-Medal-Prediction
 ┣ 📜 athlete_events.csv
 ┣ 📓 notebook.ipynb
 ┣ 📄 README.md
 ┗ 📁 images/
🚀 Future Improvements

Add more features (Year, Event, Season)

Handle class imbalance

Try advanced models (Random Forest, XGBoost)

Add cross-validation

Deploy as a web app

📊 Possible Extension

You can extend this project by:

Creating an interactive dashboard (Streamlit)

Comparing medal prediction across different Olympic eras

Adding clustering analysis

👩‍💻 Author

Maghraoui Nour
🎓 Big Data & Artificial Intelligence Student

⭐ If you like this project, feel free to give it a star on GitHub!











</p>
