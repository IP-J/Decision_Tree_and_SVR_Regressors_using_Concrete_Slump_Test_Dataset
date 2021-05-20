# Decision_Tree_and_SVR_Regressors_using_Concrete_Slump_Test_Dataset
Implementation of Decision Tree Regressor (raw, scaled) and Support Vector Regressor using Concrete Slump Test dataset

In this notebook, we will train and test two decision tree regressors(raw and scaled) and a support vector regressor.

The UCI Machine Learning Repository webpage below is a Concrete Slump Test dataset: https://archive.ics.uci.edu/ml/datasets/Concrete+Slump+Test
suitable for testing the performance of regressors. The data file slump test.data has 11 columns, including 7 input columns and 3 output columns. 
In this project, we will try to use the 7 input columns to predict the last output column (Compressive Strength (28-day)(Mpa)). So the feature dimension is 7.

The tasks done in this notebook are as follows.
1. Reading in the data file, showing a plot of the data for visualisation.
2. Implementing three regressors:
 a decision tree regressor trained on the raw features;
 a decision tree regressor trained on the scaled features computed by StandardScaler;
 a support vector regressor trained on the same scaled features above.
For the two DT regressors, 'criterion' is set to 'mse' and 'grid search' is used to experiment with two more hyperparameters, each of which has 3 values. 
For the support vector regressor, 'kernel', 'C', 'gamma', 'max_iter' hyperparameters, each with 2 to 3 values are chosen.
3. The mean squared error of the prediction of each regressor from the 3-fold cross validation is calculated as output and the performance of these regressors is compared.

