# 🧠 Multi-Class Text Classification with Deep Learning

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Latest-yellow)
![Status](https://img.shields.io/badge/Status-Complete-green)

A comprehensive Natural Language Processing (NLP) project comparing traditional Machine Learning approaches with various Deep Neural Network architectures for multi-class text classification.

## 🚀 Project Overview

This project explores the performance of different word representation techniques and model architectures on a Question-Answer classification dataset. The goal is to classify text into predefined categories using a rigorous experimental pipeline.

### Key Features
- **Exploratory Data Analysis (EDA):** Deep dive into dataset characteristics.
- **Advanced Preprocessing:** Text cleaning, stopword removal, and lemmatization.
- **Word Representations:** 
  - **TF-IDF** (Term Frequency-Inverse Document Frequency)
  - **Skip-gram Word2Vec** (Dense Embeddings)
- **Model Architectures:**
  - **Machine Learning:** Random Forest
  - **Deep Learning:** DNN, RNN, GRU, LSTM, Bi-RNN, Bi-GRU, Bi-LSTM

## 🛠️ Tech Stack

*   **Language:** Python
*   **Libraries:** 
    *   `pandas`, `numpy` (Data Manipulation)
    *   `matplotlib`, `seaborn` (Visualization)
    *   `nltk`, `re` (Text Processing)
    *   `scikit-learn` (ML Models & Metrics)
    *   `tensorflow`, `keras` (Deep Learning)
    *   `gensim` (Word Embeddings)

## 📊 Experiments & Results

We conducted extensive experiments to compare models. The pipeline includes:

1.  **Baseline:** TF-IDF + Random Forest
2.  **Dense Neural Networks:** TF-IDF + DNN
3.  **Sequence Models:** Word2Vec (Skip-gram) + RNN variants (Simple, GRU, LSTM)
4.  **Bidirectional Models:** Capturing context from both directions.

## 📂 Repository Structure

```
├── Fall 2025 - CSE440 Lab Project.pdf  # Project Requirements
├── project_notebook.ipynb              # Main Analysis Notebook
├── train.csv                           # Training Dataset
├── test.csv                            # Testing Dataset
├── INSTRUCTIONS.md                     # Detailed run guide
└── README.md                           # This file
```

## 🤝 Contribution
This project is part of the CSE440 course.

---
*Created with ❤️ for NLP*
