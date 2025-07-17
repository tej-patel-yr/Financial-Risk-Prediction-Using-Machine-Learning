# Financial Risk Prediction with ML
*Predicting Fraud, Subscriptions & Loan Defaults*

## 📌 Quick Overview
This project builds real-world ML models to solve three banking problems:
1. **Fraud Detection** → Flag suspicious transactions *(98.4% accuracy)*
2. **Banking Subscriptions** → Predict customer sign-ups *(92.9% accuracy)*
3. **Loan Defaults** → Identify risky borrowers *(93.4% accuracy)*

**Why it matters**: These models help banks save money, reduce risk, and target customers better.

## 📂 Files & Structure


## 🔍 What's Inside?

### 1. Fraud Detection
- **Goal**: Catch fake transactions before they cost money
- **Data**: 3,075 transactions (amount, merchant details, etc.)
- **Best Model**: **Logistic Regression (StatsModels)**
  - Accuracy: **98.4%**
  - Catches **95% of fraud cases** (recall)

### 2. Banking Subscriptions
- **Goal**: Find customers likely to sign up for services
- **Data**: 45,211 customers (age, job, contact history, etc.)
- **Best Model**: **XGBoost Random Forest**
  - Accuracy: **92.9%**

### 3. Loan Default Prediction
- **Goal**: Avoid lending to people who won't repay
- **Data**: 32,581 loans (income, loan amount, etc.)
- **Best Model**: **XGBoost Random Forest**
  - Accuracy: **93.4%**
  - Correctly flags **72% of risky loans** (recall)

## 🛠️ How It Works
1. **Data Cleaning**:
   - Fixed missing values (filled with averages)
   - Removed duplicates & outliers
2. **Preprocessing**:
   - Converted categories to numbers (one-hot encoding)
   - Scaled all numbers to 0-1 range (normalization)
3. **Model Training**:
   - Tested Random Forest (Scikit-learn vs. XGBoost) and Logistic Regression (Scikit-learn vs. StatsModels)
4. **Evaluation**:
   - Picked best model based on accuracy, precision, recall

## 🚀 How to Run
1. **Install Python libraries**:
   ```bash
   pip install pandas scikit-learn xgboost statsmodels jupyter
