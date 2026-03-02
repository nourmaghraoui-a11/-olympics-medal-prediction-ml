# Olympic Medal Prediction

A comprehensive data science project analyzing Olympic athlete data to predict medal performance using machine learning classification techniques.

---

## Project Overview

This project demonstrates a complete data science pipeline including data preprocessing, exploratory analysis, feature engineering, and predictive modeling. The objective is to classify whether an Olympic athlete will win a medal based on demographic and competition characteristics.

**Key Components:**
- Data Cleaning & Preprocessing
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Machine Learning Classification

**Data Source:** [Kaggle – Olympic Athlete Events Dataset](# Olympic Medal Prediction

A comprehensive data science project analyzing Olympic athlete data to predict medal performance using machine learning classification techniques.

---

## Project Overview

This project demonstrates a complete data science pipeline including data preprocessing, exploratory analysis, feature engineering, and predictive modeling. The objective is to classify whether an Olympic athlete will win a medal based on demographic and competition characteristics.

**Key Components:**
- Data Cleaning & Preprocessing
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Machine Learning Classification

**Data Source:** [Kaggle – Olympic Athlete Events Dataset](https://www.kaggle.com/datasets/heesoo37/olympic-history-data-1896-2016)

---

## Dataset Description

The dataset contains historical Olympic athlete information with the following features:

| Feature | Description |
|---------|---|
| **Age** | Athlete age |
| **Sex** | Male / Female |
| **Height** | Height (cm) |
| **Weight** | Weight (kg) |
| **Sport** | Sport category |
| **NOC** | Country code |
| **Year** | Olympic year |
| **Medal** | Gold / Silver / Bronze / No medal |

---

## Data Cleaning & Preprocessing

### 1. Duplicate Removal
- Identified and removed duplicate entries across all columns

### 2. Missing Value Handling
- Imputed missing Height and Weight values using median strategy
- Replaced missing Medal entries with "No medal" category

### 3. Feature Engineering
Created BMI (Body Mass Index) feature:
$$BMI = \frac{\text{Weight}}{(\text{Height}/100)^2}$$

Removed Height and Weight columns to reduce multicollinearity.

### 4. Column Removal
- Dropped redundant columns: Games, Team

### 5. Data Organization
- Sorted dataset by Age and Year
- Reset index for proper sequencing

---

## Exploratory Data Analysis

### Medal Distribution by Sex
Analyzed medal achievement rates across male and female athletes using comparative visualization.

### BMI Analysis by Medal Category
Examined BMI distribution across medal classes (Gold, Silver, Bronze) using boxplot analysis.

### Performance by Country
Identified top 20 countries by total medal count and NOC distribution.

---

## Machine Learning Model

### Target Variable
```python
df['HasMedal'] = (df['Medal'].isin(['Gold','Silver','Bronze'])).astype(int)
```
- **1** = Athlete won a medal
- **0** = Athlete did not win a medal

### Model Specifications
- **Algorithm:** Logistic Regression
- **Encoding:** OneHot Encoding for categorical features
- **Data Split:** 80% training / 20% testing
- **Framework:** Scikit-Learn Pipeline

### Features Used
- Age
- BMI
- Sex
- Sport
- NOC (National Olympic Committee)

### Model Evaluation
The model accuracy is calculated using:
```python
accuracy = model.score(X_test, y_test)
```

---

## Technology Stack

| Technology | Purpose |
|---|---|
| **Python** | Programming language |
| **Pandas** | Data manipulation and analysis |
| **NumPy** | Numerical computing |
| **Matplotlib** | Data visualization |
| **Seaborn** | Statistical visualization |
| **Scikit-learn** | Machine learning modeling |

---

## Project Structure

```
Olympic-Medal-Prediction/
├── amazon_sales_dataset.csv
├── Olympic Athletes Data Cleaning And Analysis.ipynb
└── README.md
```

---

## Future Enhancements

- Incorporate additional temporal features (Season, Event type)
- Implement class imbalance handling techniques
- Evaluate advanced algorithms (Random Forest, XGBoost, Gradient Boosting)
- Perform cross-validation analysis
- Deploy as interactive web application

## Possible Extensions

- Create interactive dashboard using Streamlit
- Conduct historical analysis across different Olympic eras
- Perform clustering analysis on athlete characteristics
- Build predictive model for medal type (Gold vs Silver vs Bronze)

---

## Author

**Maghraoui Nour**  
Big Data & Artificial Intelligence Student











</p>
)

---

## Dataset Description

The dataset contains historical Olympic athlete information with the following features:

| Feature | Description |
|---------|---|
| **Age** | Athlete age |
| **Sex** | Male / Female |
| **Height** | Height (cm) |
| **Weight** | Weight (kg) |
| **Sport** | Sport category |
| **NOC** | Country code |
| **Year** | Olympic year |
| **Medal** | Gold / Silver / Bronze / No medal |

---

## Data Cleaning & Preprocessing

### 1. Duplicate Removal
- Identified and removed duplicate entries across all columns

### 2. Missing Value Handling
- Imputed missing Height and Weight values using median strategy
- Replaced missing Medal entries with "No medal" category

### 3. Feature Engineering
Created BMI (Body Mass Index) feature:
$$BMI = \frac{\text{Weight}}{(\text{Height}/100)^2}$$

Removed Height and Weight columns to reduce multicollinearity.

### 4. Column Removal
- Dropped redundant columns: Games, Team

### 5. Data Organization
- Sorted dataset by Age and Year
- Reset index for proper sequencing

---

## Exploratory Data Analysis

### Medal Distribution by Sex
Analyzed medal achievement rates across male and female athletes using comparative visualization.

### BMI Analysis by Medal Category
Examined BMI distribution across medal classes (Gold, Silver, Bronze) using boxplot analysis.

### Performance by Country
Identified top 20 countries by total medal count and NOC distribution.

---

## Machine Learning Model

### Target Variable
```python
df['HasMedal'] = (df['Medal'].isin(['Gold','Silver','Bronze'])).astype(int)
```
- **1** = Athlete won a medal
- **0** = Athlete did not win a medal

### Model Specifications
- **Algorithm:** Logistic Regression
- **Encoding:** OneHot Encoding for categorical features
- **Data Split:** 80% training / 20% testing
- **Framework:** Scikit-Learn Pipeline

### Features Used
- Age
- BMI
- Sex
- Sport
- NOC (National Olympic Committee)

### Model Evaluation
The model accuracy is calculated using:
```python
accuracy = model.score(X_test, y_test)
```

---

## Technology Stack

| Technology | Purpose |
|---|---|
| **Python** | Programming language |
| **Pandas** | Data manipulation and analysis |
| **NumPy** | Numerical computing |
| **Matplotlib** | Data visualization |
| **Seaborn** | Statistical visualization |
| **Scikit-learn** | Machine learning modeling |

---

## Project Structure

```
Olympic-Medal-Prediction/
├── amazon_sales_dataset.csv
├── Olympic Athletes Data Cleaning And Analysis.ipynb
└── README.md
```

---

## Future Enhancements

- Incorporate additional temporal features (Season, Event type)
- Implement class imbalance handling techniques
- Evaluate advanced algorithms (Random Forest, XGBoost, Gradient Boosting)
- Perform cross-validation analysis
- Deploy as interactive web application

## Possible Extensions

- Create interactive dashboard using Streamlit
- Conduct historical analysis across different Olympic eras
- Perform clustering analysis on athlete characteristics
- Build predictive model for medal type (Gold vs Silver vs Bronze)

---

## Author

**Maghraoui Nour**  
Big Data & Artificial Intelligence Student











</p>
