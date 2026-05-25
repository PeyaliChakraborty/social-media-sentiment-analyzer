# Social Media Sentiment Analyzer

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/PeyaliChakraborty/social-media-sentiment-analyzer/blob/main/sentiment_model.ipynb)
[![Open in nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.org/github/PeyaliChakraborty/social-media-sentiment-analyzer/blob/main/sentiment_model.ipynb)

A machine learning project built to analyze and classify the sentiment of social media text (tweets, comments, and posts) into **Positive** or **Negative** categories using Natural Language Processing (NLP).

---

## 🚀 How It Works

1. **Text Vectorization:** Converts raw text into numerical features using a TF-IDF Vectorizer with bigram support (`ngram_range=(1,2)`).
2. **Pipeline:** Vectorizer and Logistic Regression are wrapped in a `sklearn Pipeline` to prevent data leakage.
3. **Classification:** Trains a Logistic Regression classifier on the TF-IDF features.
4. **Evaluation:** Uses stratified train/test split + 5-Fold Cross Validation for reliable scoring on small datasets.

---

## 📊 Results

| Metric | Score |
|---|---|
| Test Accuracy | 83% |
| Macro avg F1 | 0.83 |
| 5-Fold CV Accuracy | 0.60 (± 0.08) |

Sample predictions:
- `"I love this!"` ➔ **POSITIVE**
- `"This is terrible."` ➔ **NEGATIVE**

---

## 🛠️ Tech Stack

- **Language:** Python 3
- **Libraries:** `scikit-learn`, `pandas`, `numpy`
- **Environment:** GitHub Codespaces / Jupyter Notebook / Google Colab

---

## 💻 Setup Instructions

### Option 1 — Run in browser (no install needed)
Click the **Open in Colab** badge above.

### Option 2 — Run locally
1. Clone the repo:
```bash
   git clone https://github.com/PeyaliChakraborty/social-media-sentiment-analyzer.git
```
2. Install dependencies:
```bash
   pip install pandas numpy scikit-learn
```
3. Open `sentiment_model.ipynb` in Jupyter or VS Code.
