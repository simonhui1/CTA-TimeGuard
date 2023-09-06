# Predictive Service Delay Management for CTA Trains

![1](./images/CTA_train.jpg)

# Overview of Business Problem and Project 

I conducted a data analysis and machine learning project focused on predicting train delays for the Chicago Transit Authority (CTA). The goal was to develop a model that could anticipate delays and improve transit management. Here's an overview of the steps I took:

1. Data Collection via API Script
2. Exploratory Data Anaylsis 
3. Data Preprocessing
4. Selection of Models
5. Model Evaluation
6. Experiment with TPOT AutoML
7. Future Directions
8. Conclusion

For a more in-depth and technical workflow analysis, please refer to the [Jupyter notebook](./index_organized.ipynb). 
# Data Limitations

There was no access to historical data for this project, and the script used to collect the relevant transit data was not run on a cloud server, so there were hours where the script was not active. For more information about my script, please refer [here](./train_api_script.ipynb).

# Data Analysis on Delays

![2](./images/DPL.png)

The Green Line has the most occurences of delayed trains. Below is an image of the Green Line.

![3](./images/cta_GREEN.png)

![4](./images/DBS.png)

Station 40100 has the most delays recorded.

![5](./images/MORSE.png)

Station 40100 is Morse, which is highlighted here.

![6](./images/DPH.png)

6 PM CST is the hour with the most occurences of delayed trains.

# Currently Selected Model

XGBoost 

* XGBoost Test Set Accuracy: 0.9910268756018559
* XGBoost Test Set Precision: 0.1111111111111111
* XGBoost Test Set Recall: 0.11403508771929824
* XGBoost Test Set F1-score: 0.11255411255411256

# Conclusion

Currently, the best-performing model has subpar f1-score, precision, and recall.  However, predictive modeling is an iterative process and I will continue to refine the model until it is ready for deployment. A more technical roadmap is discussed in the Future Insights section below. 

# Future Insights 

* Feature Selection: Use TPOT or other feature selection techniques to identify the most important features and simplify the model while maintaining or even improving predictive power.

* Ensemble Methods: Consider ensemble methods, such as stacking, to combine the strengths of multiple models and improve predictive accuracy.

* Collect More Data: If possible, collect more data to improve model training. Larger datasets can help the models learn more patterns and generalize better.

* Domain Knowledge: Consult domain experts or stakeholders to gain insights into the factors affecting delays in public transportation. Their insights might lead to better feature engineering or model improvements.

* Consider Alternative Models: Experiment with alternative models, such as time series forecasting techniques, to address the temporal nature of public transportation data.
