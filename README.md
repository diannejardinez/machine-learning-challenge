# Machine Learning - Exoplanet Exploration

**Objective**: Create machine learning models capable of classifying candidate exoplanets from NASA Kepler space telescope raw dataset starting in 2009. 


**Background**:

Kepler Space Observatory had verified 1284 new exoplanets as of May 2016. As of October 2017 there are over 3000 confirmed exoplanets total. The raw dataset `exoplanet_data.csv` is a cumulative record of all observed Kepler "objects of interest."([Source](https://www.kaggle.com/nasa/kepler-exoplanet-search-results))



The models below were chosen on the basis of Binary Classification Predictive modeling where class label is predicted for a given example of input data([Source](https://machinelearningmastery.com/types-of-classification-in-machine-learning/#:~:text=Popular%20algorithms%20that%20can%20be%20used%20for%20binary%20classification%20include)). The planets would either be confirmed as a new exoplanet or not. 




## Analysis Report

Comparative to all the algorithms  below, the Random Forests and Logistic Regression are the models that reached greater than 85% accuracy, with Random Forests at 88.8%. If one were to make predictions of exoplanets from these five models, the best model would be Random Forests. However, the limitations of the accuracy scores are that there were no specific features selected or dropped when training the model so erroneous data might have been included in the Hyperparameter Tuning phase causing our test accuracy to be skewed. 

To improve accuracy the following may be considered:
- Using effective and efficient value hyperparameters when using Hyperparameter Tuning with GridSearch
- Removing features in the dataset that do not provide substance to classifying the exoplanets to reduce processing time
- Controlling the prevention of overfitting and under-fitting for each model


## Model Rank

### 1. Random Forests
- Predictive Test Accuracy: **0.888**
- Best Grid score: 0.872

![](https://github.com/diannejardinez/machine-learning-challenge/blob/master/classification-reports/Random-Forests.png)

### 2. Logistic Regression
- Predictive Test Accuracy: 0.880
- Best Grid score: 0.886

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
- Can be found in the `data-visualizations` directory









<!-- Readme for https://github.com/diannejardinez/machine-learning-, Author: Dianne Jardinez -->

