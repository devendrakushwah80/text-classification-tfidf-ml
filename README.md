# 📝 Text Classification using TF-IDF & Machine Learning

## 📌 Project Overview

This project demonstrates an end-to-end **text classification pipeline** using classical **Machine Learning algorithms** and **TF-IDF feature extraction**. The notebook covers data loading, text cleaning, exploratory analysis, feature engineering, model training, hyperparameter tuning, and model comparison using evaluation metrics.

The goal is to classify textual data into predefined **labels** using supervised learning.

---

## 🧠 Workflow Explained

### 1️⃣ Data Loading

* Dataset is loaded from `train.csv`
* Basic inspection using `head()` and `isnull()`

### 2️⃣ Exploratory Data Analysis (EDA)

* Label distribution visualization
* Class imbalance inspection

### 3️⃣ Text Preprocessing

A custom text-cleaning function is applied:

* Lowercasing
* Removing special characters
* Keeping only alphabets

### 4️⃣ Feature Engineering

* **TF-IDF Vectorizer**

  * Max features: 5000
  * N-grams: (1,2)

### 5️⃣ Model Building

Multiple ML models are trained using **Pipeline + GridSearchCV**:

* Logistic Regression
* Multinomial Naive Bayes
* Support Vector Machine (Linear)

### 6️⃣ Model Evaluation

Each model is evaluated using:

* Accuracy
* Precision
* Recall
* F1-score

Best-performing model is selected based on **F1-score**.

---

## 📊 Output

* Comparison table of all models
* Automatically selects best model
* Ready-to-use evaluation results

---

## 📁 Project Structure

```
text-classification-tfidf-ml/
│
├── text_classification_tfidf_models.ipynb
├── train.csv
├── requirements.txt
└── README.md
```

---

## ⚙️ Installation & Setup

### 1️⃣ Create Virtual Environment (Optional)

```bash
python -m venv venv
source venv/bin/activate  # Windows: venv\\Scripts\\activate
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Run Notebook

```bash
jupyter notebook
```

---

## 🚀 Future Improvements

* Use word embeddings (Word2Vec / GloVe)
* Try deep learning models (LSTM, BERT)
* Handle class imbalance with SMOTE
* Save best model using joblib

---

## 👨‍💻 Author

Devendra Kushwah

---

## ⭐ If you like this project

Give the repo a ⭐ and feel free to fork & improve!
