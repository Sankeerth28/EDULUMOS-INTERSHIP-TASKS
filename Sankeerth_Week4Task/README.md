# Fake News Detection using Machine Learning (NLP)

## Objective
The goal of this project is to build a reliable and interpretable machine learning model that can classify news articles as **Fake** or **Real** using Natural Language Processing techniques.  
Beyond accuracy, the focus is on understanding *why* a model makes a prediction.

---

## Dataset
- Source: Fake.csv and True.csv  
- Total articles: **44,898**
- Features used:
  - `title`
  - `text`
  - `subject`
- Target label:
  - `0` → Fake News  
  - `1` → Real News  

Both datasets were merged, shuffled, and labeled to avoid ordering bias.

---

## Dataset Link
The dataset used in this project (Fake.csv and True.csv) can be accessed from the link below:

[Dataset Link](https://drive.google.com/drive/folders/1uViefNaUP9xhgzR5O4xrAOWYJpuYBOjt)

The dataset contains labeled news articles categorized as fake and real, which were merged and preprocessed for model training and evaluation.

---

## Data Preparation
- Combined **title + text + subject** to preserve context and stylistic cues
- Converted text to lowercase
- Removed URLs, HTML tags, and punctuation
- Stopwords were intentionally not removed to retain important linguistic signals

---

## Models Implemented
Three machine learning models were trained and compared:

| Model | Accuracy |
|------|---------|
| Naive Bayes | 96.06% |
| Logistic Regression | 98.91% |
| Linear SVM | **99.73%** |

---

## Evaluation Metrics
Models were evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

The Linear SVM achieved the best overall performance with balanced precision and recall across both classes.

---

## Model Interpretability
Analysis of model coefficients revealed clear linguistic patterns:

**Fake News Indicators**
- Sensational terms (e.g., *video, watch, breaking*)
- Emotional and direct-address language
- Strong political polarization terms

**Real News Indicators**
- Source attribution (e.g., *Reuters, said, he said*)
- Temporal references (e.g., *on Tuesday, on Friday*)
- Formal reporting tone

This shows the model learns **writing style and credibility cues**, not just keywords.

---

## Model Validation
To ensure reliability:
- Manual sanity checks were performed on unseen examples
- Label shuffling confirmed no data leakage
- Feature ablation showed performance drops when contextual fields were removed

These checks confirm the model learned meaningful patterns.

---

## Limitations
- Satirical news can be misclassified
- Dataset source bias may inflate performance
- No deep contextual understanding (classical ML approach)

---

## Future Improvements
- Transformer-based models (BERT, RoBERTa)
- Source credibility modeling
- Temporal analysis using publication dates

---

## Conclusion
This project demonstrates how classical NLP and machine learning models can effectively detect fake news while remaining interpretable. The emphasis on validation and explanation makes the solution robust and trustworthy.

---

## Author
Intern – EduLumos Machine Learning Internship  
