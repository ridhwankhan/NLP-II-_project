# Project Instructions

## 🏃 How to Run the Project

1.  **Prerequisites**: Ensure you have Python installed along with the following libraries:
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn nltk tensorflow gensim
    ```
2.  **Data**:
    *   Ensure `train.csv` and `test.csv` are in the same directory as the notebook.
3.  **Execution**:
    *   Open `project_notebook.ipynb` in Jupyter Notebook or Google Colab.
    *   Run all cells sequentially (`Cell > Run All`).
    *   **Note**: Training Deep Learning models (especially LSTMs and GRUs) can be time-consuming. Using a GPU (like in Google Colab) is highly recommended.

## ❓ Preprocessing Justification ("WHY")

In this project, we applied several preprocessing steps. Here is the reasoning behind each:

### 1. Removing HTML Tags
**Why?** The dataset consists of raw text scraped from web sources (QA forums), containing tags like `<html>`, `<br>`, etc. These tags define structure but carry no semantic meaning relevant to the classification topic. Removing them reduces noise.

### 2. Lowercasing
**Why?** "Science" and "science" should be treated as the same token. Lowercasing normalizes the text, reducing the vocabulary size and ensuring the model doesn't treat capitalized versions of words as distinct entities.

### 3. Removing Non-Alphabetic Characters
**Why?** Punctuation and numbers often do not contribute significantly to topic classification in this context. Removing them simplifies the input space.

### 4. Stopword Removal
**Why?** Common words like "the", "is", "at" appear frequently but hold little discriminative power for classifying topics. Removing them allows the model to focus on content-rich keywords (e.g., "physics", "zebra", "equation").

### 5. Lemmatization
**Why?** Lemmatization reduces words to their base form (e.g., "running" -> "run", "stripes" -> "stripe"). This consolidates similar word forms into a single feature, effectively densifying the data and reducing the dimensionality of the TF-IDF matrix or embedding space, leading to better generalization.

## 🧪 Model Configuration

*   **TF-IDF**: Used for the Machine Learning baseline (Random Forest) and the Deep Neural Network (DNN) to provide a sparse, frequency-weighted representation.
*   **Skip-gram (Word2Vec)**: Used for all Sequence Models (RNN, GRU, LSTM). Skip-gram is chosen because it excels at capturing semantic context and predicting context words, which is valuable for understanding the nuances in Question-Answer text.
