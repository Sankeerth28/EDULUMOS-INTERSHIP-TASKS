# Task 01 – Smart Study Score Predictor

### 🎯 Objective
Predict a student's overall academic performance using demographic and preparation details from the **Students Performance** dataset.

### 📂 Dataset
Source: Kaggle – *Students Performance in Exams*  
Contains 1,000 records with attributes such as:
- Gender, Race/Ethnicity  
- Parental Level of Education  
- Lunch Type  
- Test Preparation Course  
- Math, Reading, and Writing Scores

A new feature **average_score** was created as the prediction target.

### 🧠 Approach
1. Data Cleaning and EDA  
2. One-Hot Encoding for categorical variables  
3. Train-Test Split (80 / 20)  
4. Model: **Linear Regression** (baseline)  
5. Evaluation using MAE, RMSE, R²

### 📊 Results
| Metric | Value |
|:--|--:|
| Mean Absolute Error | 10.49 |
| Root Mean Squared Error | 13.40 |
| R² Score | 0.16 |

### 📈 Insights
- Students completing test-prep courses tend to score higher.  
- Parental education level shows a mild positive influence on scores.  
- Current demographic features alone explain only a small part of performance variance.

### 🔧 Tools & Libraries
Python · Pandas · NumPy · Scikit-Learn · Matplotlib

### 🏁 Next Steps
- Try advanced models (Decision Tree, Random Forest, XGBoost).  
- Feature engineering (e.g., combine subject-score interactions).  
- Hyper-parameter tuning and cross-validation.

---

## 🧩 Step 3 — Final GitHub structure

