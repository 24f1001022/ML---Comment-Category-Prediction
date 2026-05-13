# 🚀 Comment Category Prediction using Machine Learning

> A complete end-to-end **Natural Language Processing (NLP)** and **Machine Learning** project for multi-class comment classification using TF-IDF, dimensionality reduction, feature engineering, and ensemble learning.

---

# 📌 Project Overview

This project focuses on predicting the **category/label of comments** using Machine Learning techniques.

The workflow includes:

- Data Cleaning & Preprocessing
- Exploratory Data Analysis (EDA)
- TF-IDF Feature Extraction
- Dimensionality Reduction using SVD
- Hyperparameter Tuning
- Multiple ML Models
- Ensemble Learning
- Kaggle Submission Pipeline

---

# 🎯 Problem Statement

Given a dataset containing textual comments and additional metadata, the goal is to accurately classify each comment into its corresponding category.

---

# 🧠 Models Used

| Model | Validation Score |
|---|---|
| Dummy Classifier | 0.5690 |
| Logistic Regression | **0.8988** ⭐ |
| SGD Classifier | 0.8846 |
| Multinomial Naive Bayes | 0.7195 |
| KNN + SVD | 0.8390 |
| Linear SVM | 0.7887 |
| MLP Classifier | 0.8912 |
| Soft Voting Ensemble (LR + XGBoost + LightGBM) | **0.9125** 🚀 |
---

# 🔥 Key Features

✅ Regex-based Text Cleaning  
✅ TF-IDF Vectorization  
✅ Truncated SVD for Dimensionality Reduction  
✅ Feature Engineering  
✅ Hyperparameter Tuning using GridSearchCV  
✅ Ensemble Learning (XGBoost + LightGBM + Logistic Regression)  
✅ Clean ML Pipeline  
✅ Kaggle Submission Ready  

---

# 📊 Exploratory Data Analysis (EDA)

The project includes:

- Missing Value Analysis
- Target Distribution Visualization
- Text Length Distribution
- Word Cloud Visualization
- Statistical Insights

## 🔍 Key Insights

- TF-IDF creates **high-dimensional sparse features**
- Linear models perform best on text data
- Logistic Regression achieved highest accuracy
- SVD helped reduce noise and dimensionality

---

# ⚙️ Tech Stack

## 🐍 Language
- Python

## 📚 Libraries
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- LightGBM
- SciPy
- Regex

---

# 🛠️ Machine Learning Workflow

```text
Data Loading
   ↓
EDA & Visualization
   ↓
Text Cleaning (Regex)
   ↓
Train Validation Split
   ↓
TF-IDF Feature Extraction
   ↓
Dimensionality Reduction (SVD)
   ↓
Model Training
   ↓
Hyperparameter Tuning
   ↓
Evaluation & Comparison
   ↓
Ensemble Learning
   ↓
Kaggle Submission
```

---

# 📂 Project Structure

```bash
📦 Comment-Category-Prediction
│
├── 📄 README.md
├── 📄 notebook.ipynb
├── 📄 submission.csv
│
├── 📂 images
│   ├── eda.png
│   ├── wordcloud.png
│   └── model_comparison.png
│
├── 📂 outputs
│   ├── trained_models
│   └── predictions
│
└── 📂 data
    ├── train.csv
    └── test.csv
```

---

# 📈 Best Performing Model

## 🏆 Soft Voting Ensemble (Logistic Regression + XGBoost + LightGBM)

### 🚀 Validation Score: **0.9125**

Why it performed best:

- Combined strengths of multiple models
- Logistic Regression handled sparse TF-IDF features effectively
- XGBoost captured complex feature interactions
- LightGBM improved generalization and handled class imbalance efficiently
- Soft voting reduced individual model weaknesses and improved prediction stability

---

## 🥈 Best Individual Model — Logistic Regression

### ⭐ Validation Score: **0.8988**

Why it worked well:

- TF-IDF features are sparse and high-dimensional
- Text data is mostly linearly separable
- L2 regularization helped prevent overfitting
- LBFGS solver converged efficiently on the dataset

---

# 🔍 Hyperparameter Tuning

Used:
- `GridSearchCV`
- Cross Validation (`cv=3`)
- F1 Macro Scoring

Example tuned parameters:

```python
{
    'classifier__C': [0.01, 0.1, 1, 10],
    'classifier__penalty': ['l2'],
    'classifier__solver': ['lbfgs']
}
```

---

# 🧪 Ensemble Learning

Implemented:

- XGBoost
- LightGBM
- Logistic Regression

Combined using:

```python
VotingClassifier(voting='soft')
```

Soft voting improved:
- Stability
- Generalization
- Overall prediction confidence

---

# 📌 Important Concepts Used

- TF-IDF
- Sparse Matrix
- High-Dimensional Data
- Linear Separability
- Dimensionality Reduction
- Overfitting Prevention
- Feature Engineering
- Ensemble Learning

---

# 🚀 Future Improvements

- Transformer Models (BERT)
- Deep Learning Approaches
- Advanced NLP preprocessing
- Better Ensemble Strategies

---

# 📸 Sample Visualizations

## 📊 Target Distribution
_Add your screenshot here_

## ☁️ Word Cloud
_Add your screenshot here_

## 📈 Model Comparison
_Add your screenshot here_

---

# 🏁 Kaggle Competition

This project was developed as part of a Kaggle Machine Learning competition focused on comment category prediction.

---

# 👨‍💻 Author

## Safwan Humayun

Passionate about:
- Machine Learning
- Deep Learning
- NLP
- Data Science

---

# ⭐ If you like this project

Give this repository a ⭐ and support the project!
