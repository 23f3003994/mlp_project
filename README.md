## Heavy Equipment Selling Price Prediction


The goal of this project is to build an end-to-end machine learning pipeline 
to predict the auction sale price of heavy construction equipment (bulldozers, 
excavators, motor graders etc.) given information about the machine and the sale.

**Dataset:** 138,701 auction records with 49 features including machine 
specifications, age, usage hours, equipment type, sale date and region.

**Target:** TargetValue - the sale price at auction in dollars.

**Metric:** RMSLE (Root Mean Squared Log Error) - measures prediction error 
in percentage terms. Being 10% wrong on a 10k machine and a 100k machine 
are penalised equally. This is why we train on log(price) - minimising RMSE 
in log space is mathematically equivalent to minimising RMSLE.