# Machine Learning Homework - Exoplanet Exploration

![exoplanets.jpg](Images/exoplanets.jpg)

## Background

Over a period of nine years in deep space, the NASA Kepler space telescope has been out on a planet-hunting mission to discover hidden planets outside of our solar system.

To help process this data, machine learning modelsare created, which are capable of classifying candidate exoplanets from the raw dataset.

These are the steps to build the models:

1. [Preprocess the raw data](#Preprocessing)
### Preprocess the Data

* Preprocess the dataset prior to fitting the model.
* Perform feature selection and remove unnecessary features.
* Use `MinMaxScaler` to scale the numerical data.
* Separate the data into training and testing data.

2. [Tune the models](#Tune-Model-Parameters)
### Tune Model Parameters

* Use `GridSearch` to tune model parameters.
* Tune and compare at least two different classifiers.

3. [Compare two or more models](#Evaluate-Model-Performance)
### Reporting

* Include a analysis on README that reports a comparison of each model's performance as well as a summary about findings and any assumptions based on your model (is your model good enough to predict new exoplanets? Why or why not? What would make your model be better at predicting new exoplanets?).

- - -

# Report

## Linear Support Vector Classfication ('modedl1.svc')

* After cleaning,and preparing data, Support Vector Classificaiton(SVC) method is used to analyze the NASA Kepler space data.

* After training and testing the data, it retruns 'Training Data Score: 0.8439824527942018', and 'Testing Data Score: 0.8415331807780321'.

* Model's parameters are tuned with 'GridSearchCV', then 'best_score_' goes up to '0.8680138845428944'.

## Logisitic Regression ('model2.svc')

* After cleaning, and preparing data, Logisitc Regression method is used to analyze the MASA Kepler space data.

* After training, and testing the data, it returns 'Training Data Score: 0.8512302117108526', and 'Testing Data Score: 0.847254004576659'.

* Model's parameters are tuned with 'GridSearchCV', then 'best_score_' goes up to '0.8653430384444654'.

## Final Analysis

* As seen in above results, both 'SVM' and 'Logisitc Regression' models perform very closely. The differences between two models are less than 0.01. After tuning the test parameters, their differences become three-decimal points. Therefore, both models are providing pararity results. 
- - -

## Resources

* [Exoplanet Data Source](https://www.kaggle.com/nasa/kepler-exoplanet-search-results)

* [Scikit-Learn Tutorial Part 1](https://www.youtube.com/watch?v=4PXAztQtoTg)

* [Scikit-Learn Tutorial Part 2](https://www.youtube.com/watch?v=gK43gtGh49o&t=5858s)

* [Grid Search](https://scikit-learn.org/stable/modules/grid_search.html)


