# Machine Learning - Exoplanet Exploration Analysis

**Objective**: Create machine learning models capable of classifying candidate exoplanets from NASA Kepler space telescope raw dataset 


**Background**: Kepler Space Observatory had verified 1284 new exoplanets as of May 2016. As of October 2017 there are over 3000 confirmed exoplanets total. The raw dataset `exoplanet_data.csv` is a cumulative record of all observed Kepler "objects of interest."([Source](https://www.kaggle.com/nasa/kepler-exoplanet-search-results))



The models below were chosen on the basis of Binary Classification Predictive modeling where class label is predicted for a given example of input data([Source](https://machinelearningmastery.com/types-of-classification-in-machine-learning/#:~:text=Popular%20algorithms%20that%20can%20be%20used%20for%20binary%20classification%20include)). The planets would either be confirmed as a new exoplanet or not. 




## Analysis Report

Comparative to all the algorithms  below, the Random Forests and Logistic Regression are the models that reached greater than 85% accuracy, with Random Forests at 89%. If one were to make predictions of exoplanets from these five models, the best model would be Random Forests. However, the limitations of the accuracy scores are that there were no specific features selected or dropped when training the model so erroneous data might have been included in the Hyperparameter Tuning phase causing our test accuracy to be skewed. 

To improve accuracy the following may be considered:
- Using effective and efficient value hyperparameters when using Hyperparameter Tuning with GridSearch
- Removing features in the dataset that do not provide substance to classifying the exoplanets to reduce processing time
- Controlling the prevention of overfitting and under-fitting for each model


## Model Rank

### 1. Random Forests
- Predictive Test Accuracy: **0.890**
- Best Grid score: 0.873

![](https://github.com/diannejardinez/machine-learning-challenge/blob/master/classification-reports/Random-Forests.png)

### 2. Logistic Regression
- Predictive Test Accuracy: 0.880
- Best Grid score: 0.885

![](https://github.com/diannejardinez/machine-learning-challenge/blob/master/classification-reports/Logistic-Regression.png)

### 3. Decision Trees
- Predictive Test Accuracy: 0.799
- Best Grid score: 0.790

![](https://github.com/diannejardinez/machine-learning-challenge/blob/master/classification-reports/Decision-Tree.png)

### 4. K-Nearest Neighbors(KNN)
- Predictive Test Accuracy: 0.660
- Best Grid score: 0.672

![](https://github.com/diannejardinez/machine-learning-challenge/blob/master/classification-reports/KNN.png)

### 5. Support Vector Machine(SVM)
- Predictive Test Accuracy: 0.600
- Best Grid score: 0.605

![](https://github.com/diannejardinez/machine-learning-challenge/blob/master/classification-reports/SVM.png)


## Additional Information

#### Fastest run time
- Decision Trees at 5.1 seconds with 216 fits

#### Slowest run time
- K-Nearest Neighbors(KNN) at 29.1 minutes with 28420 fits


#### Challenges
- Capturing all Hyperparameter Tuning model parameters for each model
- Run time for fitting after GridSearchCV


#### Model and Dataset Visualizations
- Extra visualizations can be found in the `data-visualizations` directory



---

# Machine Learning - Exoplanet Exploration Instructions

## Background

Over a period of nine years in deep space, the NASA Kepler space telescope has been out on a planet-hunting mission to discover hidden planets outside of our solar system.

To help process this data, you will create machine learning models capable of classifying candidate exoplanets from the raw dataset.

In this homework assignment, you will need to:

1. [Preprocess the raw data](#Preprocessing)
2. [Tune the models](#Tune-Model-Parameters)
3. [Compare two or more models](#Evaluate-Model-Performance)

- - -

## Instructions

### Preprocess the Data

* Preprocess the dataset prior to fitting the model.
* Perform feature selection and remove unnecessary features.
* Use `MinMaxScaler` to scale the numerical data.
* Separate the data into training and testing data.

### Tune Model Parameters

* Use `GridSearch` to tune model parameters.
* Tune and compare at least two different classifiers.

### Reporting

* Create a README that reports a comparison of each model's performance as well as a summary about your findings and any assumptions you can make based on your model (is your model good enough to predict new exoplanets? Why or why not? What would make your model be better at predicting new exoplanets?).

- - -

## Resources

* [Exoplanet Data Source](https://www.kaggle.com/nasa/kepler-exoplanet-search-results)

* [Scikit-Learn Tutorial Part 1](https://www.youtube.com/watch?v=4PXAztQtoTg)

* [Scikit-Learn Tutorial Part 2](https://www.youtube.com/watch?v=gK43gtGh49o&t=5858s)

* [Grid Search](https://scikit-learn.org/stable/modules/grid_search.html)

- - -

## Hints and Considerations

* Start by cleaning the data, removing unnecessary columns, and scaling the data.

* Not all variables are significant be sure to remove any insignificant variables.

* Make sure your `sklearn` package is up to date.

* Try a simple model first, and then tune the model using `GridSearch`.

- - -


##### © 2019 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
