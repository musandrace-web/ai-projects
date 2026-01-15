# Project Title
**Email Spam Classifier**  
*Final project for the Building AI course*

---

## Summary
This project builds a simple machine learning model to classify emails as spam or not spam. It demonstrates preprocessing, supervised learning, and evaluation metrics while highlighting challenges in imbalanced datasets.

---

## Background
Spam emails are a common problem in digital communication, often cluttering inboxes and posing security risks. This project addresses these challenges by providing a model to automatically detect spam. Key motivations include:

- How imbalanced datasets affect model performance  
- Why accuracy alone can be misleading  
- The importance of precision, recall, and F1-score  

---

## How is it used?
Users can feed the model a collection of emails, and it classifies each email as spam or legitimate. The solution is useful in:

- Email clients or filtering systems  
- Organizations that want to reduce spam and phishing emails  
- Individuals who want to protect personal email accounts  

The model is most effective on preprocessed text data and in environments where rare events (spam) need careful detection.

```python
# Example code for predicting email spam
from email_classifier import SpamClassifier

model = SpamClassifier()
prediction = model.predict("sample_email.txt")
print(prediction)
```
# Data Sources and AI Methods

## Dataset
- **Size**: 1000 emails  
  - 990 legitimate  
  - 10 spam  

## Data Split
- Training and test sets maintain the same spam-to-legitimate ratio.

## Preprocessing
- Tokenization  
- Bag-of-words representation  
- Text normalization  

## Model
- **Primary**: Logistic Regression  
- **Baseline**: Majority-class classifier (always predicts legitimate)  

## Evaluation Metrics
- Accuracy  
- Precision  
- Recall  
- F1-score  

---

# Results

---

# Insights
- Accuracy can be misleading in imbalanced datasets.  
- Precision and recall provide a clearer picture of model usefulness.  
- Detecting rare events like spam requires careful metric selection.  

---

# Challenges
- Imbalanced dataset makes detecting spam harder.  
- The model may misclassify rare but important emails.  
- **Ethical consideration**: Blocking legitimate emails may affect users.  

---

# What Next?
- Explore more advanced models:  
  - Naive Bayes  
  - Random Forest  
  - Neural Networks  
- Use larger and more balanced datasets.  
- Apply TF-IDF and word embeddings for richer feature representation.  
- Potentially integrate into email clients for real-time spam detection.  

---

# Acknowledgments
- Inspiration and guidance from the *Building AI* course at University of Helsinki.  
- Dataset sources and open access materials.  
- Licensed under the MIT License. Full copyright retained by the author.
