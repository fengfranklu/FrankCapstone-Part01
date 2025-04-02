# FrankCapstone-Part01
This is the Part 1 of the Capstone Project for Machine Learning Certificate

## Overview

In this application, you will explore a dataset from Kaggle. The original dataset contained information on over 30,000 movies, spanning 60 years of data. We aim to explore this dataset and determine if a movie rating can be accurately predicted.



## Business Understanding

From a business perspective, if we can predict a movie's rating based on the provided feature values, it will give the movie producer guidance on which movies to produce and which features to prioritize. As such, the company can potentially generate more revenue for each movie they make.



## Notebook

[https://github.com/fengfranklu/FrankCapstone-Part01/blob/main/Frank_Capstone01.ipynb](https://github.com/fengfranklu/FrankCapstone-Part01/blob/main/Frank_Capstone01.ipynb)



## Evaluation and Conclusion

With our initial linear regression and Random Forest Models, the training and predictions are not sufficiently accurate to be helpful. My thinking is that the cleaned-up input features are not very predictive of the rating result. To enhance this prediction model, I would like to incorporate movie budget information into the input features and explore additional models to further develop this study.  Eliminating the budget factor from the input feature due to the presence of significant missing data points may be a mistake in this study.  I want to explore the dataset more to see if any other meaningful info can be derived. 

|      |                Model | R^2 Score | Accuracy (%) | Mean Squared Error | Root MSE | Mean Absolute Error |
| ---: | -------------------: | --------: | -----------: | -----------------: | -------: | ------------------- |
|    0 |    Linear Regression |    0.0453 |       4.5255 |             1.0405 |   1.0201 | 0.7945              |
|    1 | Random Forest (Base) |    0.3470 |      34.6990 |             0.7117 |   0.8436 | 0.6376              |

|      |             Features | Importance (%) |
| ---: | -------------------: | -------------- |
|    0 |             duration | 13.56          |
|   11 |               genres | 13.17          |
|    4 |           Movie_Link | 8.61           |
|   12 |            languages | 7.17           |
|   10 | production_companies | 6.29           |
|    2 |                votes | 6.16           |
|    6 |            directors | 5.95           |
|    3 |          description | 5.94           |
|    7 |                stars | 5.89           |
|    5 |              writers | 5.72           |
|    8 |     countries_origin | 5.43           |
|    9 |    filming_locations | 5.04           |
|   14 |         release_date | 4.44           |
|   13 |                 year | 4.17           |
|    1 |                  MPA | 2.46           |
