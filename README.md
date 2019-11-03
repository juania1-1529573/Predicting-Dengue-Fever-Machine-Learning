In this project we use machine learning to predict dengue cases. 

First we load the data provided on DrivenData. We separete the data into two subsets, San Juan and Iquitos, becasue in the previous assignment, we found that the geographical data for each city are very different. We then fill in the empty values with the last valid value (`ffill`). 

We then create a new feature about the difference in temperature because, based on our domain knowledge, incubation period of the virus shortens in warmer temperatures and we want to keep track of the change in temperature and see how it affects the total dengue cases. 

After that, we train and test four types of machine learning models to predict the data. we use
* KNeighborsRegressor
* RandomForestRegressor
* GradientBoostingRegressor
* Support Vector Regressior
and determine the performance of the model by calculating the negative mean absolute error (`neg_mean_absolute_error`). The negative mean absolute error shows that Support Vector Regressor is our most accurate model.

Finally, we create some auxiliary visualizations to see the distribution of errors, We also compare the predicted value and the actual value and compare the performance for different parameters for our Support Vector Regressor model.
