# ds17_tv_shows
+ [Flat File](https://github.com/mosheharary/ds17_tv_shows/blob/main//tv_flat_file.ipynb)
+ [Data Prep](https://github.com/mosheharary/ds17_tv_shows/blob/main/tv_data_prep.ipynb)
+ [Data Clean](https://github.com/mosheharary/ds17_tv_shows/blob/main/tv_data_cleansing.ipynb)
+ [Feature selection](https://github.com/mosheharary/ds17_tv_shows/blob/main/tv_feature_selection.ipynb)
+ [Model selection  and Prediction](https://github.com/mosheharary/ds17_tv_shows/blob/main/tv_model_selection_and_prediction.ipynb)


Data Preparation:

Loaded the dataset and checked for missing values.
Dropped irrelevant columns and filled missing values with the median.

Selected the top 10 features using SelectKBest.

Regression Models Used:

+ Linear Regression
+ Ridge Regression
+ Lasso Regression
+ Decision Tree
+ Random Forest
+ Gradient Boosting
+ Support Vector Regression

Model Evaluation:

Each model was evaluated using Mean Squared Error (MSE) and R-squared (R²) metrics.
Plots were generated to show the difference between predicted and actual values for each model.
Feature Selection:

The selected features for the models were: 
  'number_of_episodes'
  'vote_count'
  'vote_average'
  'genres_Drama'
  'genres_Sci-Fi_and_Fantasy'
  'genres_Action_and_Adventure'
  'genres_Comedy'
  'genres_Animation'
  'genres_Soap'
  'genres_UnKnown'

Hyperparameter Tuning:

Conducted for the GradientBoostingRegressor model using GridSearchCV.
Best parameters found: {'max_depth': 5, 'min_samples_split': 2, 'n_estimators': 50}

Best GradientBoostingRegressor 
  MSE: 1690.6698589381194
  R2: -0.18620335062826854


