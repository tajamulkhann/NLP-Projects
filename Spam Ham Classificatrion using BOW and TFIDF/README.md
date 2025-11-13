# ✉️ Spam vs Ham Classification using BOW & TF-IDF

A natural-language-processing project focused on classifying SMS/email messages into spam (unwanted) or ham (legitimate) using Bag-of-Words and TF-IDF feature techniques.

---

## 📌 Project Overview

This project implements a full pipeline: collecting a message dataset labelled spam/ham, preprocessing text, engineering features using Bag-of-Words (BOW) and TF-IDF vectorisation, training classification models (e.g., Logistic Regression, Naive Bayes), evaluating performance, and delivering insights about how text features differentiate spam from ham. The goal is to build a model that accurately flags unwanted messages and understand key linguistic indicators of spam.

---

## 🧰 Tech Stack

* **Language:** Python
* **Libraries:** pandas, numpy, scikit-learn, matplotlib, seaborn, NLTK or spaCy for NLP preprocessing
* **Environment:** Jupyter Notebook / Google Colab

---

## 🔄 Workflow Summary

### 1. Data Collection & Pre-processing

* Load labelled dataset of messages (SMS or email) with target column “spam” or “ham”.
* Clean text: convert to lowercase, remove punctuation/stop-words, optionally lemmatise or stem.
* Split dataset into training and test sets (e.g., 80/20) with stratification on target.

### 2. Feature Engineering: BOW & TF-IDF

* Vectorise text using:

  * **Bag-of-Words (CountVectorizer)**
  * **TF-IDF (TfidfVectorizer)**
* Optionally limit vocabulary size (e.g., top 5000 words) and trim rare words
* Stack or compare both feature representations for modelling

### 3. Modelling

* Build baseline classification models:

  * **Logistic Regression**
  * **Naive Bayes (MultinomialNB)**
* Optionally explore tree-based methods (Random Forest) or ensemble
* Train models on BOW and TF-IDF features; compare performance

### 4. Evaluation

* Metrics used: Accuracy, Precision, Recall, F1-Score, Confusion Matrix
* Pay special attention to recall on spam class (missing spam is costly)
* Compare how BOW vs TF-IDF features affect performance

### 5. Insights & Application

* Identify which words/features strongly signal spam (e.g., “free”, “win”, “click”) versus ham features.
* Provide recommendations: filtering rules, alerting system, UI for message classification.
* Demonstrate how feature engineering and representation techniques impact classification quality.

---

## 📁 Project Structure

```
Spam-Ham-Classification-BOW-TFIDF/
│── data/
│   ├── raw/
│   └── processed/
│── notebooks/
│   └── spam_ham_classification.ipynb
│── src/
│   ├── preprocess.py
│   ├── features.py
│   ├── model.py
│   └── evaluate.py
│── README.md
│── requirements.txt
```

---

## 📈 Key Findings

* TF-IDF features delivered slightly stronger performance than raw BOW in capturing discriminative terms and reducing noise.
* Words such as **“free”**, **“win”**, **“offer”**, **“now”** were among top signals for spam class; while common ham messages contained more personal/context words.
* Logistic Regression and Naive Bayes performed well given the relatively straightforward feature space and task; tree-based models had limited incremental benefit.
* Proper preprocessing (removal of stop-words, lemmatisation) improved classification stability across BOW and TF-IDF feature sets.

---

## 🚀 Future Improvements

* Move from BOW/TF-IDF to more advanced text representations (e.g., word embeddings, transformer-based features) to capture context better.
* Expand to multi-language spam detection and more diverse message formats (email, social-media DMs, chat).
* Deploy model via web or mobile app: input message → classification result + confidence score.
* Integrate model into messaging system for real-time spam filtering and user-feedback loop.
* Add explainability (LIME/SHAP) to show users why a message was flagged as spam.

---

## 🧑‍💻 Author

**[Tajamul Khan](https://www.linkedin.com/in/tajamulkhann/) – Data Scientist & AI Engineer**

---

## Let's Connect <img src="https://github.com/JayantGoel001/JayantGoel001/blob/master/GIF/Handshake.gif" height="30px" style="max-width:100%;">

<div align="center">

<a href="https://www.linkedin.com/in/tajamulkhann/">
<img src="https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white">
</a>
<a href="https://www.instagram.com/tajamul.datascientist/" target="_blank">
<img src="https://img.shields.io/badge/Instagram-%23E4405F.svg?style=for-the-badge&logo=instagram&logoColor=white">
</a>
<a href="https://topmate.io/tajamulkhan" target="_blank">
<img src="https://img.shields.io/badge/Topmate-FF0000?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAxMDAgMTAwIj48Y2lyY2xlIGN4PSI1MCIgY3k9IjUwIiByPSI0MCIgZmlsbD0id2hpdGUiLz48L3N2Zz4=&logoColor=white">
</a>
<a href="https://www.whatsapp.com/channel/0029VaYs05jJkK7JKCesw42f">
<img src="https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white">
</a>
<a href="https://t.me/tajamul_khan">
<img src="https://img.shields.io/badge/Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white">
</a>
<a href="https://substack.com/@tajamulkhan">
<img src="https://img.shields.io/badge/Substack-%23006f5c.svg?style=for-the-badge&logo=substack&logoColor=FF6719">
</a>
<a href="https://www.kaggle.com/tajamulkhan">
<img src="https://img.shields.io/badge/Kaggle-035a7d?style=for-the-badge&logo=kaggle&logoColor=white">
</a>
<a href="https://github.com/tajamulkhann">
<img src="https://img.shields.io/badge/Github-12100E?style=for-the-badge&logo=github&logoColor=white">
</a>
<a href="https://medium.com/@tajamulkhan">
<img src="https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white">
</a>
<a href="https://www.youtube.com">
<img src="https://img.shields.io/badge/YouTube-%23FF0000.svg?style=for-the-badge&logo=YouTube&logoColor=white">
</a>
</div>
