---
layout: project
title: Audience Segmentation with XGBoost
subtitle: Classified users from ad-event data for targeted marketing
---
Developed an Audience Segmentation model using XGBoost to classify premium users from 250K+ ad-event records and 15 behavioral features. The project began with exploratory data analysis to examine feature distributions, handle missing values, and address class imbalance. The model achieved an AUC (Area Under the ROC Curve) of 0.79, reflecting strong ability to distinguish between premium and non-premium users. AUC summarizes how well the model ranks positive instances over negatives across all classification thresholds. It is especially valuable in imbalanced datasets where accuracy may be misleading. 

Boosting is an ensemble learning technique that combines multiple weak learners (typically decision trees) in sequence, where each model focuses on correcting the errors of the previous one. XGBoost (Extreme Gradient Boosting) is an optimized implementation that supports regularization, handles missing data efficiently, and scales well to large datasets. Its main strength lies in high performance on structured data and robust generalization. A potential drawback is that, despite built-in regularization, XGBoost can still overfit if hyperparameters are not carefully tuned.

<a href="https://github.com/jaivardhanschauhan/MLprojects/tree/main/highvalue_users" target="_blank" class="button">Code</a>
