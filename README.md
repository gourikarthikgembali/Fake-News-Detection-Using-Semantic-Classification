# Fake News Detection (Semantic Classification)

A concise pipeline to classify news articles as **True** or **Fake** using:

- Text preprocessing (cleaning, tokenization, PoS via spaCy)
- Feature extraction (vectorization; compatible with Word2Vec or traditional methods)
- Supervised learning for semantic classification
- Evaluation with accuracy, precision, recall, and F1

---

## ✨ What the project does
- Loads **True.csv** and **Fake.csv** (title, text, date)
- Performs **EDA** on train/validation splits
- Builds features and trains a classifier
- Reports metrics and visualizations

---

## 📁 Data
- `True.csv`: 21,417 true news items (title, text, date)
- `Fake.csv`: 23,502 fake news items (title, text, date)

> The notebook/script expects these files in the working directory. Place them alongside the code before running.

---

## 🧠 Key components (as implemented in the script)
- **Data Preparation & Understanding**
- **Text Preprocessing** (regex, tokenization, optional lemmatization)
- **Train/Validation Split**
- **EDA** (word clouds, frequency plots)
- **Feature Extraction** (vectorizers; Word2Vec optional extension)
- **Model Training & Evaluation** (metrics: accuracy, precision, recall, F1)

---

## 🛠 Requirements
- Python ≥ 3.8
- pandas, numpy, nltk, spaCy, seaborn, matplotlib, plotly, scikit-learn, tqdm, wordcloud

Install:
```bash
pip install pandas numpy nltk spacy seaborn matplotlib plotly scikit-learn tqdm wordcloud
python -m spacy download en_core_web_sm
```

---

## ▶️ How to run
1. Ensure `True.csv` and `Fake.csv` are present in the working directory.
2. Run the script/notebook:
   - Load data → preprocess text → split into train/validation
   - Extract features → train the classifier
   - Evaluate and visualize results

---

## 🔧 Notes & Extensions
- You can swap vectorization to **Word2Vec** (gensim) or **TF‑IDF**.
- Try multiple models (Logistic Regression, SVM, LinearSVC, etc.) and compare metrics.
- Add robust preprocessing: stopword removal, lemmatization, punctuation handling.

---

## 📄 License
Educational use.
