# Twitter-NLP-Financial-News-Sentiment

**CS M148 Final Project**
**Authors: Skylesha Marcel, Jacob Kadari, Euleena Trinh, Nathan Truong**

---

## Overview
The project classifies **financial sentiment** (Bearish, Bullish, Neutral) from Twitter posts and news headlines using **BERT and FinancialBERT embeddings** and various ML models.

---

## Dataset
The Twitter Financial News Sentiment Database (Hugging Face):
  - Training: 9,938 samples
  - Testing: 2,486 samples
  - Labels: Bearish (0), Bullish (1), Neutral (2)

Stratified sampling was used to maintain class balances.

---

## Methodology
  - Text preprocessing (URLs, emojis, stopwords, normalization)
  - BERT and FinancialBERT embeddings (768 dimensions)
  - Dimensionality reduction through PCA
  - Evaluation Models:
      - Logistic Regression using keywords
      - **Random Forest (best performing)**
      - Neural Networks

---

## Results
**Random Forest (10-Fold CV):**
  - Accuracy: **0.739**
  - Macro F1: **0.739**
  - AUC (per class): **0.84-0.86**

This model had good generalization across all classes.

---

## Files
  - `CSM148_Project_Report.pdf`: Full report
  - `notebooks/` - EDA, Models, & Analysis


