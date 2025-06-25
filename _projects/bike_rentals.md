---
layout: project
title: Customer demand in the ride sharing industry
subtitle: Predicting bike rentals using decision tree based models
---

<script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>

This project involved analyzing and forecasting bike rental demand using the <a href="https://archive.ics.uci.edu/dataset/275/bike+sharing+dataset"> UCI Bike Sharing dataset <a/> (Washington D.C. system, 2011-2012). The workflow included detailed EDA, time series analysis, feature engineering, and predictive modeling with decision trees in Python. Exploratory analysis revealed clear seasonal and hourly patterns in customer demand. For instance, rentals peaked in summer months and during morning/evening commute hours, with notable drops in extreme weather. Total rentals varied by season, weekday, and hour, with higher demand on weekdays compared to weekends. <br/>

Using scikit-learn’s DecisionTreeRegressor, the project built interpretable regression models to predict rental counts based on features like hour of day, weekday, season, and weather conditions. The model effectively captured key trends and allowed visualization of decision paths affecting customer demand. A Random Forest model performed predictive modelign with a R<sup>2</sup> of 0.92, showcasing high performance over the bike sharing dataset. Overall, the project demonstrates how tree based models can help forecast short-term demand for shared mobility services. In turn, such models can enable better fleet management, dynamic pricing, and resource planning in ride-sharing platforms.

<a href="https://github.com/jaivardhanschauhan/MLprojects/tree/main/BikeRentals" target="_blank" class="button">Code</a>















