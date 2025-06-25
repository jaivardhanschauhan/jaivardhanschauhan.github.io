---
layout: project
title: Analyzing NYC restaurant market using customer reviews
subtitle: Logistic regression and business classification in R
---
In this project, I used logistic regression in R to classify New York City restaurants as either “luxury” or “low-end” based on customer reviews and key restaurant attributes. The objective was to understand which factors contribute to a restaurant’s perceived elegance and to build a predictive model that can generalize to new cases. The model used four explanatory variables - Food, Service, Decor, and Location. Because logistic regression is non-linear, we used Average Marginal Effects (AME) to interpret the impact of each variable on classification outcomes. 

The analysis showed that a one unit increase in decor rating reduces the probability of a restaurant being low-end by an average of 8.5%. Likewise, improving food ratings by one unit lowers that probability by 6.37%. Both effects were statistically significant. On the other hand, variables such as location (east of 5th Ave) and service rating were not statistically significant. These results align with intuition: restaurants investing in better decor and food quality are more likely to be perceived as luxury, while lower-end restaurants may cut corners on food quality and ambiance. 

<a href="https://github.com/jaivardhanschauhan/statisticalinference/blob/main/RestaurantClassifier/RestaurantClassifier.md" target="_blank" class="button">Code</a>
