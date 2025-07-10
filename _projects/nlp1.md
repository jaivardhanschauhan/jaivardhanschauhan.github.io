---
layout: project
title: Natural Language Processing for Academic Scoring
subtitle: Essay Scoring with TF-IDF and Sentence Embeddings
---

We built a machine learning pipeline to predict student essay scores using natural language processing. The goal was to automate the grading process by training a regression model on student-written essays. We started with traditional preprocessing and handcrafted features and later compared these to deep sentence embeddings using the Universal Sentence Encoder.

The first step was text cleaning. We converted all essay text to lowercase, removed punctuation and stopwords using NLTK’s English stopword list, and lemmatized the tokens to reduce them to their base form. This helped standardize the data and reduce noise. Next, we engineered features from the cleaned text. We started with a unigram Bag-of-Words model using scikit-learn’s CountVectorizer and later switched to TF-IDF to weigh more informative terms higher. To reduce noise, we excluded rare words that appeared in fewer than 3 documents and very common words that appeared in over 90% of documents. We visualized the top 20 TF-IDF features, which gave us insights into the most influential words across essays. We also tested adding bigrams and dataset-specific stopwords like “essay” and “prompt” to refine our feature set.

We trained two types of models on these features. The first was Ridge regression, a regularized linear model. We used cross-validation to tune the regularization coefficient. It performed adequately for essays with mid-range scores but struggled with very low and very high scores. The second model was a Random Forest regressor, which we chose for its ability to capture non-linear relationships. We tuned the number of trees and maximum depth. This model performed better than Ridge overall and was more robust across different score ranges. We compared both models using R² scores and found that the Random Forest consistently outperformed Ridge.

After evaluating traditional models, we moved to deep learning. We used the Universal Sentence Encoder from TensorFlow Hub to convert each essay into a dense embedding that captures the semantic meaning of the text. We passed these embeddings into the Random Forest model, which had already performed nicely on TF-IDF features. The model trained on sentence embeddings outperformed the one trained on TF-IDF features, especially on edge cases where essays had very high or very low scores. This confirmed that using pretrained embeddings can significantly improve performance in NLP tasks like essay grading.

Overall, we found that careful preprocessing and feature engineering can produce decent results, but deep transfer learning methods like sentence embeddings lead to stronger performance with less manual tuning. The Random Forest model, when paired with dense embeddings, offered the best results in our experiments. This project showed a clear advantage of combining traditional supervised learning with modern NLP tools to build practical, scalable solutions for NLP tasks.

<a href="https://github.com/jaivardhanschauhan/nlp-work/tree/master/Predicting%20Essay%20Scores" target="_blank" class="button">Code</a>
