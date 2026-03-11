# Customer Churn Prediction Project

##  Project Overview
This project predicts customer churn using machine learning classification models. Customer churn means when customers stop doing business with a company.

## Dataset
- **Source:** Kaggle Telco Customer Churn Dataset
- **Rows:** 7,043 customers
- **Columns:** 21 features
- **Target Variable:** Churn (Yes/No) - 26.5% churn rate

##  Technologies Used
- Python 3.x
- Pandas, NumPy (Data Processing)
- Matplotlib, Seaborn (Visualizations)
- Scikit-learn (Machine Learning)

##  Project Pipeline

### 1. Data Loading & Exploration
- Loaded telecom customer data
- Checked data types and missing values
- Analyzed churn distribution

### 2. Exploratory Data Analysis (EDA)
- **Churn Distribution:** 73.5% No churn, 26.5% Churn
- **Key Insights:**
  - Senior citizens have higher churn rate
  - Month-to-month contracts show more churn
  - Fiber optic users churn more
  - Electronic check payment users churn more

### 3. Data Preprocessing
- Handled missing values
- Encoded categorical variables (One-Hot Encoding)
- Scaled numerical features (StandardScaler)
- Train-test split (80-20)

### 4. Model Training
Two classification models were trained:
- **Logistic Regression**
- **K-Nearest Neighbors (KNN)**

### 5. Model Evaluation
Models were evaluated using:
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

##  Results

| Model | Accuracy | Precision | Recall | F1-Score |
|-------|----------|-----------|--------|----------|
| Logistic Regression | 0.8034 | 0.6721 | 0.5487 | 0.6042 |
| KNN | 0.7821 | 0.6245 | 0.5213 | 0.5682 |

**Best Model:** Logistic Regression with 80.34% accuracy

## Key Findings
1. **Tenure** is the most important factor - newer customers churn more
2. **Contract type** matters - month-to-month customers at highest risk
3. **Monthly charges** - higher charges lead to more churn
4. **Internet service** - Fiber optic users churn more than DSL

## Project Structure