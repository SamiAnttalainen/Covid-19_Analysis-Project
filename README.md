# Covid-19 Project

The goal of this project is to analyze some Covid-19 data and try to create useful models that can predict, classify or cluster data and gain new insights from it.

## Analysis part

In the first analysis part we are first going to explore the data and handle missing data. Rows that have missing data are dropped from the dataframe to reduce noise. Then we are going to do some small data analysis about Covid-19 in Finland and try to find some interesting information.

In the second part of the analysis we are going to feature engineer more features to the dataframe and do some analysis about them. We are trying to come up with features that might help us with the classification modeling.

In the last part we are going to add polynomial features to the dataframe and then use PCA to analyze all the feature importances.

## Regression part

In the regression part we are just going to test some multi regression modeling for the base dataset without added features to keep the model as simple as possible. The goal is just to test the regression modeling and optimization, because the dataset is about different countries, so we cannot make any useful continuous predictions with the data, because different countries have their own nuances and forcing all the countries to a simplified regression would give us very misleading information. We are going to use XGBoost Regressor model to do the multi linear regression modelling and HyperOpt optimization to optimize some of the hyperparameters for the XGB model.

## Classification part

The classification part is the main modelling in this project, because the data fits our classification modelling criteria. In this part we are going to use XGB Classifier as classification model and HyperOpt optimizer as hyperparameter optimizer.

 We are first going to build a base classification model and test how it performs on the base dataset. Then we are going to do some feature engineering and check which features help the most with the classification task.

In the second part of the classification task we are going to start optimizing the model with different hyperparameters and also drop some noisy data from the dataset to prevent under- and overfitting.

In the last part we are going to add polynomial features to the dataset to see if they help the model with the classification.

## Cluster Analysis part

In the cluster analysis part we are just going to clean the data first and then perform simple Elbow method to figure out which k-value is the best for the Kmeans clustering algorithm and then analysing the clusters.

In this part we are going to perform very simple cluster analysis to the base data between **'Recovered'** and **'Deaths'** features and try to find out if there are some distinct groups between the countries, which can be clustered. Finally we are going to do some analysis about the clustered groups.
