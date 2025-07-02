# 📰 Fake News Detection using Logistic Regression

This project is a Machine Learning-based **Fake News Detection** system that classifies a given news article as either **Fake** or **Real**. It uses **Natural Language Processing (NLP)** techniques for text transformation and a **Logistic Regression** classifier for prediction. The model is deployed using **Streamlit**, enabling users to interactively test news articles in real-time.

---

## 🧠 Objective

The goal of this project is to combat misinformation by building a lightweight, fast, and interpretable machine learning model that identifies fake news based on article content.

---

## 📌 Features

- Simple and interactive Streamlit UI  
- Real-time fake/real news prediction  
- Utilizes TF-IDF for vectorization  
- Efficient and interpretable Logistic Regression model  
- High accuracy and low latency  

---

## 📊 Dataset

The dataset used is the [Fake and Real News Dataset](https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset) from Kaggle.

It contains:  
- **True.csv**: Real news articles  
- **Fake.csv**: Fake news articles  

Each entry includes `title`, `text`, and `subject` fields which are preprocessed and combined for model training.

---

## ⚙️ Model Overview

1. **Text Preprocessing**:  
   - Lowercasing, punctuation removal, and tokenization  
   - Optional stopword removal  

2. **Feature Extraction**:  
   - TF-IDF vectorizer to convert text into numerical features  

3. **Model Training**:  
   - Logistic Regression classifier trained on processed features  

4. **Deployment**:  
   - The model (`lr_model.jb`) and vectorizer (`vectorizer.jb`) are saved using Joblib  
   - Streamlit frontend enables real-time text input and classification  

---

## 🛠️ How to Use

1. Clone the repository  
2. Install the required packages from `requirements.txt`  
3. Run the app:  
   ```bash
   streamlit run app.py
## ✅ Example Result

**Input:**  
`"The government announced a new policy on renewable energy..."`

**Output:**  
✅ The News is Real!

---

## 📚 Technologies Used

- Python  
- Scikit-learn  
- Joblib  
- Streamlit  
- Pandas / Numpy  
- TF-IDF (from `sklearn.feature_extraction.text`)

---

## 📌 Conclusion

This project demonstrates how simple and interpretable ML models, when paired with effective NLP techniques, can deliver practical solutions to modern-day problems like fake news detection. Future improvements could involve:

- Training advanced models like BERT  
- Including URL-based features  
- Expanding dataset diversity
