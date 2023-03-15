# Retail-Sales-Prediction

<p align="center">
  <img width="460" height="300" src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/b2/Ro%C3%9Fmann-Markt_in_Berlin.jpg/1024px-Ro%C3%9Fmann-Markt_in_Berlin.jpg">
</p>

Rossmann operates over 3,000 drug stores in 7 European countries. Currently, Rossmann store managers are tasked with predicting their daily sales for up to six weeks in advance. Store sales are influenced by many factors, including promotions, competition, school and state holidays, seasonality, and locality. With thousands of individual managers predicting sales based on their unique circumstances, the accuracy of results can be quite varied. My work includes various plots and graphs , visualizations , feature engineering , ensemble techniques , different ML algorithms with their respective parameter tuning , analysis and trends . Predictions are of 6 weeks of daily sales for 1,115 stores located across Germany.

In this project, the Kaggle Rossman challenge is being taken on. The goal is to predict the Sales of a given store on a given day. Model performance is evaluated on the root mean absolute percentage error (MAPE).


The dataset consists of two csv files: store.csv and train.csv

Data Files:

train.csv holds info about each store. store.csv holds the sales info per day for each store.

The repo contains main.py that runs the main script from step one until the end.


## 1. Business Problem.
Rossmann operates over 3,000 drug stores in 7 European countries. Currently, Rossmann store managers are tasked with predicting their daily sales for up to six weeks in advance. Store sales are influenced by many factors, including promotions, competition, school and state holidays, seasonality, and locality. With thousands of individual managers predicting sales based on their unique circumstances, the accuracy of results can be quite varied.

## 2. Solution Strategy
My strategy to solve this challenge was:

Step 01: Data Description: Use statistics metrics to identify data distributions.

Step 02: Feature Engineering: Derive new attributes based on the original variables to better describe the phenomenon that will be modeled.

Step 03: Exploratory Data Analysis: Explore the data to find insights and better understand the impact of variables on model learning.

Step 04: Feature Selection: Selection of the most significant attributes for training the model.

Step 05: Machine Learning Modelling: Machine Learning model training.

Step 06: Hyperparameter Fine Tunning: hoose the best values for each of the parameters of the model selected from the previous step.

Step 07: Convert Model Performance to Business Values: Convert the performance of the Machine Learning model into a business result.



## 3.Machine Learning Model Implementation and performance
At this stage models used : *Linear Regression, *Lasso Regression, *Decision Tree,*Random Forest Regressor

               						     Testing score(adjusted_r2_score)
			Linear Regression			         0.7067
			
			Lasso Regression			         0.7068
			
			Decision Tree                                    0.8273
			
			Random Forest    	             	         0.8420





## 4. Conclusion

1. By Linear modeling on our dataset we infer that the MSE was *1559270.5*, RMSE was *1248.71*, R2 was *0.70215*, adjusted R2 was *0.70212*.

2. From Lasso regression analysis R2 was *0.70237*, adjusted R2 was *0.70349* which is a clear indication that our model does not overfit.

3. By decision tree analysis we found that MSE: 0.00384, MAE: 0.04868, RMSE : 0.06199, R2 : 0.85395,adjusted_r2_score :0.8272

4. By Random forest analysis our model improved and the R2 was ***0.8657***, MSE : 0.00269, RMSE : 0.05188, MAE : 0.04048, adjusted_r2_score : 0.8419
