# Task 02 - AI Health Analyst: Heart Disease Prediction

## Overview
This project implements a machine learning model to predict the presence of heart disease using patient health metrics. The model uses **Logistic Regression** for binary classification.

## Dataset
- **Source**: Heart Disease Dataset from Kaggle (UCI Heart Disease Dataset)
- **Size**: 1,025 patient records
- **Features**: 13 health metrics (age, sex, chest pain type, blood pressure, cholesterol, etc.)
- **Target**: Binary classification (0 = No Disease, 1 = Disease Present)

## Project Structure
```
Sankeerth_Week2Task/
├── task02_notebook.ipynb    # Main Jupyter notebook with complete analysis
└── README.md                 # This file
```

## Notebook Sections
1. **Problem Statement** - Introduction to heart disease prediction
2. **Dataset Overview** - Feature descriptions and data exploration
3. **EDA (Exploratory Data Analysis)** - Visualizations and correlation analysis
4. **Data Preprocessing** - Feature scaling and train-test split
5. **Model Training** - Logistic Regression training
6. **Evaluation** - Performance metrics and confusion matrix
7. **Conclusion** - Key findings and insights

## Model Performance
- **Accuracy**: 80.98%
- **Precision**: 76.19%
- **Recall**: 91.43% (Critical for medical diagnosis)
- **F1-Score**: 83.12%

## Key Features
- ✅ Complete end-to-end ML pipeline
- ✅ Comprehensive EDA with visualizations
- ✅ Feature scaling (StandardScaler)
- ✅ Multiple evaluation metrics
- ✅ Confusion matrix visualization
- ✅ Feature importance analysis
- ✅ Training vs Test comparison

## Technologies Used
- **Python 3.10+**
- **Pandas** - Data manipulation
- **NumPy** - Numerical operations
- **Scikit-Learn** - Machine learning
- **Matplotlib & Seaborn** - Data visualization

## How to Run
1. Install required packages:
   ```bash
   pip install jupyter pandas numpy scikit-learn matplotlib seaborn
   ```

2. Open the notebook:
   ```bash
   jupyter notebook task02_notebook.ipynb
   ```

3. Run all cells sequentially (Cell → Run All)

## Key Learnings
1. **Feature Scaling is Critical** - Logistic Regression requires normalized features
2. **Accuracy Alone is Insufficient** - Must consider precision, recall, and F1-score
3. **Recall is Critical in Medical Diagnosis** - Missing disease cases is costly
4. **Balanced Dataset** - ~51% disease cases vs ~49% no disease

## Results Summary
- **True Positives**: 96 (Correctly identified disease cases)
- **True Negatives**: 70 (Correctly identified no disease)
- **False Positives**: 30 (Flagged healthy as disease)
- **False Negatives**: 9 (Missed disease cases)

The model achieves **91.43% recall**, meaning it successfully identifies most disease cases, which is crucial in medical diagnosis where missing a disease can have serious consequences.

## Future Improvements
- Ensemble methods (Random Forest, XGBoost)
- Hyperparameter tuning
- Cross-validation for robust estimates
- Feature engineering
- Deep learning approaches

## Disclaimer
This model is for **educational purposes only** and should NOT be used as a substitute for professional medical diagnosis.

## Author
Sankeerth - Week 2 Internship Task
