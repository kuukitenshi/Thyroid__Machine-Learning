# Thyroid - Machine Learning

This project was a collaborative effort involving two more students for our ```Machine Learning``` subject.

In this project, a version of the ```thyroid0387``` dataset was analyzed, which is a subset of a dataset largest, the ```"Thyroid Disease dataset"```, containing data from patients with thyroid disease, including information demographics, thyroid hormone levels, and diagnostic information.
In this way, knowing the dataset, our tasks were to investigate the best possible models, which allow us to achieve our objectives, that is, to obtain with confidence the answer to whether we can predict the diagnosis, the age and sex of a subject, given the remaining attributes, as well as determining what the most significant features in the best models obtained.

That was implemented in ```python``` using ```Jupyter Notebook```.

All the functionalities were successfully implemented, and we received a ```very high score```.

---
## Data processing

In order to analyze the dataset in question, we needed to process its data:

- Categorize the classes present in the target;
- Delete the Record Identification column;
- Replacement of "?" values;
- Replacing column types;
- Parse columns to int;
- Elimination of outliers associated with age;
- Elimination of the hypopituitary feature;
- Treatment of missing values ​​in the TSH, T3, TT4, T4U, FTI, TBG columns;
- Performing a One Hot Encoder in the referral source column;
- Elimination of NaN’s;
- Eliminating duplicate lines.

---
## Feature Selection

In order to carry out an extensive analysis of the different models for objectives O1 and O2, we carried out a ```Forward Feature Selection``` until the 8 best features of each model,  allowing us a general analysis of each model with the features that bring them greater benefits, and is also justified as it allows to reduce the number of features in the model, making it simpler.

---
## Modeling Results

### Classification:
1. K-Nearest Neighbors (KNeighborsClassifier)
2. Support Vector Classifier (SVC)
3. Guassian Naive Bayes (GaussianNB)
4. Rede neuronal (MLPClassifier)
5. Adaptive Boosting Ensemble (AdaBoostClassifier)
6. Random Forest Ensemble (RandomForestClassifier)
7. Árvores de decisão (DecisionTreeClassifier)
8. eXtreme Gradient Boosting Ensemble (XGBoostClassifier)

### Regression:
1. Random Forest (RandomForestRegressor)
2. K-Nearest Neighbors (KNeighborsRegressor)
3. Árvores de decisão (DecisionTreeRegressor)
4. Regressão Linear (LinearRegression)
5. Support Vector Regressor Linear (LinearSVR)
6. Cross Validation Ridge (RidgeCV)
7. Cross Validation Elastic Net (ElasticNetCV)
8. Cross Validation Lasso (LassoCV)

---
## Hyperparameters Tuning

Tuning was carried out for the 3 models chosen in the previous section, using a ```Grid Search```, selecting the appropriate hyperparameters for each model.