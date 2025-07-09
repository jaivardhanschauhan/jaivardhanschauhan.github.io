---
layout: project
title: UW Datathon DubsTech'24
subtitle: Machine Learning for inventory and marketing decisions
---
The “Retail: Accelerating the Sales of Urban Edge Apparel” datathon asked teams to mine a decade-long transactional file (~89K Orders, 2013-24) and explain how the clothing brand could grow sales. We tackled questions on shifting purchase habits, seasonality, basket size, product health, customer segments, and regional performance. 

Our team, Data Vizperts, started by filtering out cancelled or unpaid orders, checking data types, fixing nulls, and deriving new calendar fields such as order quarter and weekend flag. We log-scaled prices and quantities, applied Min-Max scaling, and confirmed normalised distributions with quick plots. Everything after December 2022 stayed unseen for testing. Clear annual peaks made a seasonal ARIMA the right tool; a grid search found the best variant, which scored about 30 USD MAE and roughly 82 % accuracy on the hold-out set. We then refit that model on the full history to forecast revenue through 2026 and repeated the same loop for every product and client to flag rising stars. Coupled with dashboards that track basket size, product winners, and regional demand, these forecasts support clear calls on inventory timing, holiday campaigns, and SKU focus.

<a href="https://github.com/jaivardhanschauhan/UW-Datathon24" target="_blank" class="button">Code</a>
