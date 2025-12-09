# Task 01 – Smart Study Score Predictor

### 🎯 Objective
Predict a student’s **average academic score** using demographic and preparation details from the Students Performance dataset.

---

### 📂 Dataset
**Source:** Kaggle – *Students Performance in Exams*  
**Records:** 1000 students  
**Columns:**
- Gender  
- Race/Ethnicity  
- Parental level of education  
- Lunch type  
- Test preparation course  
- Math score, Reading score, Writing score  

A new feature **`average_score`** was created as the prediction target.

---

### 🧠 Approach
1. Data Cleaning and EDA  
2. One-Hot Encoding for categorical variables  
3. Train/Test split (80 / 20)  
4. Model → **Linear Regression**  
5. Evaluation → MAE, RMSE, R²  

---

### 📊 Results
| Metric | Value |
|:--|--:|
| Mean Absolute Error | 10.49 |
| Root Mean Squared Error | 13.40 |
| R² Score | 0.16 |

---

### 📈 Insights
- Students who completed test-preparation courses scored higher on average.  
- Parental education level had a moderate positive effect on scores.  
- Current features explain limited variance (≈ 16 %), so further feature engineering is needed.

---

### 🛠️ Tools & Libraries
Python · Pandas · NumPy · Scikit-Learn · Matplotlib

---

### 🏁 Next Steps
- Try advanced models (Decision Tree, Random Forest, XGBoost).  
- Perform hyper-parameter tuning and cross-validation.  
- Add feature scaling and interaction features to improve R².

---

### EDA Insights Summary
- The dataset contains 1000 students with no missing values.
- Math, reading, and writing scores are strongly correlated.
- Students with “standard” lunch and completed test-preparation course score higher.
- Parental education level shows a moderate upward trend in average score.
- The distribution of average scores is roughly normal, centered around 65–70.

---

**Author:** Sankeerth (@Sankeerth28)  
**Internship:** EduLumos – Machine Learning Internship (Week 1)
