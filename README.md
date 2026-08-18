# 🎬 Movie Genre Classification

## 📌 Project Overview

This project uses **Machine Learning and Natural Language Processing (NLP)** to classify movies into different genres based on their **title and plot description**.

The project uses **TF-IDF Vectorization** to convert movie text into numerical features and **Logistic Regression** for multi-class genre classification.

---

## 🎯 Objective

The main objective of this project is to build a machine learning model that can automatically predict the genre of a movie from its title and description.

---

## 📊 Dataset

The dataset contains movie information with the following columns:

* **ID** – Unique movie identifier
* **TITLE** – Movie title
* **GENRE** – Movie genre
* **DESCRIPTION** – Movie plot/description

### Dataset Statistics

* **Total Movies:** 54,214
* **Number of Genres:** 27
* **Missing Values:** 0
* **Duplicate Rows:** 0

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* TF-IDF
* Logistic Regression
* Joblib

---

## 🔄 Project Workflow

1. Dataset loading
2. Data exploration
3. Missing value checking
4. Duplicate checking
5. Genre distribution visualization
6. Text preprocessing
7. Combining movie title and description
8. Train-test splitting
9. TF-IDF feature extraction
10. Logistic Regression model training
11. Model evaluation
12. Confusion matrix visualization
13. Movie genre prediction
14. Model and vectorizer saving

---

## 🤖 Machine Learning Model

### Logistic Regression

Logistic Regression was used as the classification algorithm because it performs well for text classification problems and supports multi-class classification.

### Feature Extraction

**TF-IDF (Term Frequency-Inverse Document Frequency)** was used to transform movie text into numerical features.

The model uses:

* Movie Title
* Movie Description
* Unigrams and Bigrams
* English stop-word removal

---

## 📈 Model Performance

### Baseline Model

**Accuracy:** 57.99%

### Improved Model

**Accuracy:** 59.81%

**Improvement:** 1.82 percentage points

The improved model uses both **movie title + description**, along with enhanced TF-IDF settings.

---

## 🎬 Example Prediction

### Input

**Movie Title:** The Haunted House

**Description:**
A group of friends enters an abandoned house and discovers a terrifying supernatural presence.

### Prediction

**Predicted Genre:** Horror

---

## 💾 Saved Model Files

The trained model and TF-IDF vectorizer were saved using Joblib:

```text
movie_genre_model.pkl
movie_genre_tfidf.pkl
```

---

## 📁 Project Structure

```text
Movie_Genre_Classification/
│
├── Movie_Genre_Classification.ipynb
├── README.md
├── movie_genre_model.pkl
├── movie_genre_tfidf.pkl
│
└── Genre Classification Dataset.csv/
    ├── train_data.txt
    ├── test_data.txt
    ├── test_data_solution.txt
    └── description.txt
```

---

## 🚀 Future Improvements

* Use advanced NLP models such as BERT
* Handle class imbalance using appropriate techniques
* Hyperparameter tuning
* Experiment with Linear SVM and Naive Bayes
* Build a web application using Streamlit
* Improve performance on rare movie genres

---

## 👨‍💻 Project Purpose

This project was developed as part of a **Machine Learning Internship** to demonstrate practical skills in:

* Machine Learning
* Natural Language Processing
* Text Classification
* Data Preprocessing
* Model Evaluation
* Python Programming

---

## ⭐ Conclusion

The project successfully demonstrates how machine learning and NLP can be used to automatically classify movie genres from textual information.

The final Logistic Regression model achieved approximately **59.81% accuracy** on the test set and successfully predicted movie genres from new descriptions.
