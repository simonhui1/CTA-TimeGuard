# Predictive Service Delay Management for CTA Trains

![1](./images/CTA_train.jpg)

# Overview of Business Problem and Project 

Chicago has the second-largest transit system in the United States, and yet, it is still plagued with constant delays. The goal of this project is to arrive at a functioning predictive model to predict delays for commuting CTA trains in Chicago. 

# Data Limitations

There was no access to historical data for this project, and the script used to collect the relevant transit data was not run on a cloud server, so there were hours where the script was not active. For more information about my script, please refer [here](./train_api_script.ipynb).

# Data Analysis

![2](./images/DPL.png)

The Green Line has the most occurences of delayed trains. Below is an image of the Green Line.

![3](./images/cta_GREEN.png)

![4](./images/DBS.png)

Station 40100 has the most delays recorded.

![5](./images/MORSE.png)

Station 40100 is Morse, which is highlighted here.

![6](./images/DPH.png)

6 PM CST is the hour with the most occurences of delayed trains.

# Selected Model

Decision Tree

* 11.85% precision
* 14.04% recall
* F1-score of 0.113

# Conclusion and Future Insights 

The best-performing model that came out of this project, has subpar precision, recall, and F1-score. However, this is an iterative process and I will continue finetuning hyperparameters to improve the performance of this model and hopefully deploy it on an app. Nonetheless, there are several recommendations to the commuters of Chicago:

* Prepare in advance
* Download available train-tracking apps
* Use alternative commuting methods, such as biking
