# Book Recommendation Classifier
a minimal implementation of a book recommender using Naive Bayes from scikit-learn 

---

## Overview

This project uses a dataset of books to build a binary classifier that predicts whether a book is recommended.

Features include:
- Number of pages
- Number of ratings
- Number of text reviews

---

## Technologies

- Python 3
- Pandas, NumPy
- scikit-learn

---

## 📂 Dataset

The dataset used is a cleaned CSV version of [Goodreads book ratings]([https://example.com](https://www.kaggle.com/datasets/jealousleopard/goodreadsbooks))  

---

## 🧠 Machine Learning Approach

- **Model**: Multinomial Naive Bayes
- **Problem type**: Binary classification
- **Target**: `average_rating > 3.8 → recommended (1), else not recommended (0)`
- **Preprocessing**:
  - Filled missing values
  - Log-transformed skewed numerical features (`log1p`)

---

## 📊 Results

- **Accuracy**: ~70%
- Model heavily improved after applying `log1p` to numerical features.
