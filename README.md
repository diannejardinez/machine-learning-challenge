# Machine Learning - Exoplanet Exploration

**Objective**: Create machine learning models capable of classifying candidate exoplanets from NASA Kelper space telescope raw dataset starting at 2009. 


**Background**:

Kepler Space Observatory had verified 1284 new exoplanets as of May 2016. As of October 2017 there are over 3000 confirmed exoplanets total. The raw dataset `exoplanet_data.csv` is a cumulative record of all observed Kepler "objects of interest" — basically, all of the approximately 10,000 exoplanet candidates Kepler has taken observations on [Source](https://www.kaggle.com/nasa/kepler-exoplanet-search-results)



The models below were chosen on the basis of Classification Predictive modeling where class label is predicted for a given example of input data([Source](https://machinelearningmastery.com/types-of-classification-in-machine-learning/#:~:text=Imbalanced%20Classification-,Classification%20Predictive%20Modeling,it%20is%20spam%20or%20not.)). The planets would either confirmed as a new exoplanet  or not. 




## Analysis Report

Model Ranking showing grid score, classification report, and are ranked by Test Accuracy.

Comparative to all the algorithms  below, the Random Forests and Logistic Regression are the models that reached greater than 85% accuracy, with Random Forests at 88.8%

### Random Forest
- Predictive Test Accuracy: **0.888**
- Best Grid score: 0.872

![](https://github.com/diannejardinez/machine-learning-challenge/blob/master/classification-reports/Random-Forests.png)

Logistic Regression
- Predictive Test Accuracy: 0.880
- Best Grid score: 0.886

![](https://github.com/diannejardinez/machine-learning-challenge/blob/master/classification-reports/Logistic-Regression.png)

Decision Tree
- Predictive Test Accuracy: 0.799
- Best Grid score: 0.790

![](https://github.com/diannejardinez/machine-learning-challenge/blob/master/classification-reports/Decision-Tree.png)

KNN
- Predictive Test Accuracy: 0.660
- Best Grid score: 0.672

![](https://github.com/diannejardinez/machine-learning-challenge/blob/master/classification-reports/KNN.png)

SVM
- Predictive Test Accuracy: 0.600
- Best Grid score: 0.605

![](https://github.com/diannejardinez/machine-learning-challenge/blob/master/classification-reports/SVM.png)


Fastest run time
- Decision Tree at 5.1 seconds with 216 fits

Slowest run time
- K-Nearest Neighbors(KNN) at 29.1 minutes with 28420 fits


There could be a better way at increasing the accuracy for each model by doing more research on the appropriate hyperarameters for Hyperparameter Tuning for each model.


Challenges
- Hyperparameter Tuning model parameters for each model
- Run time for fitting after GridSearchCV













<!-- Readme for https://github.com/diannejardinez/machine-learning-, Author: Dianne Jardinez -->