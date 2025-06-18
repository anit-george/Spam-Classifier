# 📧 Spam Classifier (Email/SMS Detection)

A machine learning project that classifies text messages as **Spam** or **Ham** using NLP and a Naive Bayes classifier. It includes a training pipeline, serialized model and vectorizer, and a Flask app (`app.py`) for deployment.

🔗 **Try it locally** with the included `app.py`.

---

## 🚀 Features

- Text preprocessing and label encoding
- NLP feature extraction using **CountVectorizer**
- Model training with **Multinomial Naive Bayes**
- Evaluation using confusion matrix and accuracy score
- Flask app for real-time message prediction
- Includes pickled model and vectorizer

---

## 🧾 Dataset

- File: `spam.csv`
- Size: 5,572 messages
- Columns Used:
  - `v1`: Label (`ham` or `spam`)
  - `v2`: Text message

---

## 🧠 ML Pipeline

| Step         | Description                     |
|--------------|----------------------------------|
| 🧹 Cleaning   | Label encoding (`ham` = 0, `spam` = 1) |
| 🏗 Vectorizer | `CountVectorizer` for Bag-of-Words   |
| 🧪 Model      | `MultinomialNB` (Naive Bayes)        |
| 📈 Evaluation | Accuracy score, confusion matrix     |

---

## 📁 Repository Structure

```
Spam-Classifier/
├── Dataset/
│   └── spam.csv
├── notebook/
│   └── email classifier.ipynb
├── app.py                    # Flask app for prediction
├── model.pk1                # Saved trained model
├── vectorizer.pk1           # Saved CountVectorizer
├── README.md
```

---

## ⚙️ How to Run Locally

### 1. Clone the repository

```bash
git clone https://github.com/Anit-George/Spam-Classifier.git
cd Spam-Classifier
```

### 2. Install dependencies

Create a virtual environment (optional but recommended):

```bash
pip install -r requirements.txt
```

> If you don’t have `requirements.txt`, install manually:
```bash
pip install pandas numpy scikit-learn flask
```

### 3. Run the Flask app

```bash
python app.py
```

Then go to `http://127.0.0.1:5000/` in your browser.

---


## 📊 Sample Evaluation Metrics

- Accuracy: **~98%**
- Model: Multinomial Naive Bayes
- Feature count: ~8,500 unique words

---

## 🔮 Future Improvements

- Use TF-IDF instead of CountVectorizer
- Clean stopwords, punctuation, and symbols
- Add live demo with Streamlit or Flask UI
- Save prediction history with timestamps

---

## 👨‍💻 Author

**Anit George**  
🔗 [GitHub](https://github.com/Anit-George)

---
