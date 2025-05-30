# 📩 Spam SMS Detection

## 🔍 Objective

The objective of this project is to build a Machine Learning model that can accurately classify SMS messages as **spam** or **ham** (legitimate). This can help users automatically filter unwanted messages and improve digital communication hygiene.

---

## 📁 Dataset

- **Source**: [UCI SMS Spam Collection Dataset](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset)
- **Description**: A labeled collection of 5,574 SMS messages tagged as `ham` or `spam`.
- **Format**:
  - `v1`: Message label (`ham` or `spam`)
  - `v2`: Raw text message

---

## 🛠️ Technologies & Libraries Used

- **Languages**: Python
- **Libraries**:
  - `pandas`, `numpy`, `matplotlib`, `seaborn`
  - `scikit-learn`
  - `nltk`, `re`, `string`
  - `wordcloud`

---

## 🧹 Data Preprocessing

- Removed irrelevant columns and duplicate entries
- Encoded categorical labels (`ham` → 0, `spam` → 1)
- Cleaned and normalized text (lowercasing, stopwords removal, lemmatization)
- Engineered features like:
  - Message length
  - Word count, unique word count
  - Stopword and punctuation counts
  - Hashtags and mentions

---

## 📊 Exploratory Data Analysis (EDA)

- Analyzed class distribution using bar and pie charts
- Investigated message length and other feature distributions
- Generated **WordClouds** for spam and ham messages
- Visualized feature correlation heatmap and pair plots

---

## 🧠 Text Vectorization

- Used **TF-IDF** (`TfidfVectorizer`) for converting text to numerical format
- Limited to top 3000 features for efficiency

---

## 🤖 Models Used

The following models were trained and evaluated:

| Model                     | Accuracy | Precision | Recall | F1 Score |
|--------------------------|----------|-----------|--------|----------|
| Logistic Regression      | 95.36%   | 94.50%    | 71.03% | 81.10%   |
| SVC (Support Vector)     | 97.97%   | 98.43%    | 86.90% | 92.31%   |
| Gaussian Naive Bayes     | 87.23%   | 52.81%    | 84.13% | 64.89%   |
| Multinomial Naive Bayes  | 97.48%   | 98.37%    | 83.45% | 90.30%   |
| **Bernoulli Naive Bayes**| **98.06%**| **96.30%**| **89.65%**| **92.85%**|

✅ **Best Performing Model**: **Bernoulli Naive Bayes**

---

## 📈 Evaluation

- Evaluated using accuracy, precision, recall, and F1-score
- Visualized confusion matrix via heatmap
- Bernoulli Naive Bayes achieved **98% accuracy** with a balanced F1-score
