# 📝 Sentiment Analysis on Amazon Product Reviews

## 📌 Project Summary

This project builds a **multi-class sentiment classifier** to categorize Amazon-style product reviews as **positive**, **neutral**, or **negative**. Mock data is generated using the `Faker` library, and multiple models are trained to evaluate classification performance.

---

## 🎯 Objectives

* Generate synthetic review data
* Preprocess text (cleaning, tokenization, stopword removal)
* Train sentiment classifiers: Naive Bayes and LSTM
* Evaluate performance with classification reports and confusion matrix
* Visualize sentiment patterns using word clouds

---

## 🛠 Key Components

### 1. **Data Generation**

* 5,000 synthetic reviews generated using `Faker`
* Balanced distribution across 3 sentiment labels

### 2. **Preprocessing**

* Cleaned text using regex, tokenization, and stopword removal (NLTK)
* Split into train/test sets (80/20 stratified)

### 3. **Modeling**

#### 🧪 Naive Bayes (with TF-IDF)

* GridSearchCV used for hyperparameter tuning
* TF-IDF features extracted with n-grams and stopword filtering

#### 🧠 LSTM Model (Keras)

* Tokenized and padded sequences
* Simple LSTM architecture: Embedding → LSTM → Dropout → Dense layers
* Trained with `sparse_categorical_crossentropy` loss

---

## 📊 Evaluation

* **Naive Bayes**

  * Accuracy ≈ 34%
  * Good recall for neutral class; poor for positive/negative

* **LSTM**

  * Accuracy stagnated (\~35%); likely due to data simplicity

* **Confusion Matrix**: Visualized misclassifications

* **Classification Report**: Showed precision, recall, F1-score

* **Word Clouds**: Highlighted frequent terms by sentiment

---

## 📦 Dependencies

* `pandas`, `numpy`, `nltk`
* `scikit-learn`
* `faker`, `matplotlib`, `seaborn`
* `keras`, `tensorflow`
* `wordcloud`

---

## 📁 Project Structure

```
.
├── sentiment_analysis_notebook.ipynb
├── Task2_README.md
├── data/ (optional, for real datasets)
└── models/ (optional, for saved models)
```

---

## 🚧 Limitations & Notes

* LSTM and Naive Bayes underperform due to **synthetic randomness** of fake reviews
* For real-world accuracy, use authentic labeled reviews (e.g., from Amazon)