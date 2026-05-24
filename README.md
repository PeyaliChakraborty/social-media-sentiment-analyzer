# Social Media Sentiment Analyzer

A machine learning project built to analyze and classify the sentiment of social media text (tweets, comments, and posts) into **Positive** or **Negative** categories using Natural Language Processing (NLP).

---

## 🚀 How It Works
1. **Text Vectorization:** Converts raw text strings into numerical features using a $TF-IDF$ (Term Frequency-Inverse Document Frequency) Vectorizer.
2. **Classification:** Trains a **Logistic Regression** classifier to map those textual features to emotional sentiments based on historical patterns.

## 📊 Sample Results
The model successfully flags text sentiment:
* *"This is the best pencil I have used!"* ➔ **POSITIVE**
* *"I am so frustrated, it broke immediately."* ➔ **NEGATIVE**

## 🛠️ Tech Stack
* **Language:** Python 3
* **Libraries:** `scikit-learn`, `pandas`, `numpy`
* **Environment:** GitHub Codespaces / Jupyter Notebook

## 💻 Setup Instructions
1. Open this repository inside a **GitHub Codespace**.
2. Run the following command in the terminal to install dependencies:
   ```bash
   pip install pandas numpy scikit-learn
   ```
