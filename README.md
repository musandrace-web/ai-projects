# AI Project: Email Spam Classifier

## Summary
This project implements a simple email spam classifier using supervised machine learning.  
A Logistic Regression model is trained on a highly imbalanced dataset to highlight the limitations of accuracy as a performance metric and demonstrate the importance of precision, recall, and F1-score when detecting rare events such as spam.

## Introduction
This project was developed as part of the **Building AI course**.  
The aim is to design a simple machine learning model that can classify emails as either **spam** or **not spam**.  
The project demonstrates fundamental concepts in **supervised learning**, **data preprocessing**, and **evaluation metrics**.

## Motivation
Spam emails are a persistent problem in digital communication. Building a classifier helps illustrate:

- How imbalanced datasets affect model performance  
- Why accuracy alone is misleading in skewed distributions  
- The importance of precision, recall, and F1-score  

## Dataset
- **Size:** 1000 emails  
- **Distribution:** 990 legitimate, 10 spam  
- **Split:** Training and test sets maintain the same ratio of spam to legitimate emails  

## Methodology

### Preprocessing
- Tokenization and bag-of-words representation  
- Normalization of text features  

### Model
- Logistic Regression classifier  
- Baseline comparison against a majority-class classifier (always predicts legitimate)  

### Evaluation Metrics
- Accuracy  
- Precision  
- Recall  
- F1-score  

## Results
- **Baseline accuracy:** 99% (majority-class classifier)  
- **Logistic Regression:**
  - Accuracy: 97%  
  - Precision (spam): 0.80  
  - Recall (spam): 0.70  
  - F1-score: 0.75  

## Insights
- Accuracy is misleading in imbalanced datasets  
- Precision and recall provide a clearer picture of model usefulness  
- Detecting rare events (spam) requires careful metric selection  

## Future Work
- Explore advanced models (Naive Bayes, Random Forest, Neural Networks)  
- Use larger and more balanced datasets  
- Apply TF-IDF and word embeddings for richer feature representation  

## License
This project is licensed under the **MIT License**.  
You retain full copyright of your work.
