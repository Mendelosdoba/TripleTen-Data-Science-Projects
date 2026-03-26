
# 🎬 Movie Review Sentiment Classification

## 📖 Project Description
This project builds a machine learning model to classify movie reviews as **positive** or **negative**.  
The goal is to simulate a real-world system that can automatically analyze user feedback.

---

## 🎯 Objectives
- Clean and preprocess text data  
- Convert text into numerical features (TF-IDF)  
- Train classification models  
- Evaluate performance using metrics like F1-score and ROC-AUC  

---

## 📂 Dataset
The dataset contains movie reviews labeled as:
- Positive  
- Negative  

Each review is processed and transformed into features for model training.

---

## ⚙️ Methods
- Text cleaning (removing punctuation, lowercasing)
- Lemmatization using spaCy
- TF-IDF vectorization
- Model training:
 
 
## 🤖 Modeling Approach

To solve the sentiment classification task, several models and preprocessing techniques were explored and compared.

First, a **baseline model** was created to establish a reference point for performance.

Next, a pipeline using **NLTK for text preprocessing**, combined with **TF-IDF vectorization** and a **Logistic Regression model**, was implemented. This provided a solid starting point for handling textual data.

To improve text representation, **spaCy** was then used for more advanced preprocessing and lemmatization. This was again paired with **TF-IDF** and **Logistic Regression**, allowing for a direct comparison with the NLTK-based approach.

Finally, to capture more complex patterns in the data, a **LightGBM classifier** was trained using spaCy-processed text and TF-IDF features. This model aimed to improve performance by leveraging a more powerful algorithm.

All models were evaluated and compared to determine the most effective combination of preprocessing and classification techniques.  - 

---

## 📊 Evaluation Metrics
- F1 Score  
- ROC-AUC  
- Precision & Recall  

---

## 🚀 Results
The model successfully classifies reviews with strong performance, showing that simple models can perform well with proper preprocessing and feature engineering.

---

## 🛠️ Tools & Libraries
- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- spaCy  

---

## 📌 Conclusion
This project demonstrates how natural language processing and machine learning can be used to solve real-world classification problems effectively.
