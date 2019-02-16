# House Prices: Advanced Regression Techniques
This is the Final Project for the course in **Fundamentals in Data Science (2018-2019)**

This project of [Kaggle](https://www.kaggle.com/c/house-prices-advanced-regression-techniques) is about the prediction in house-sale
prices and an inauguration in basics of machine learning.

![](https://storage.googleapis.com/kaggle-competitions/kaggle/5407/media/housesbanner.png)


*kaggle name: [JasonTarzan](https://www.kaggle.com/jasontarzan)*

*final_score: 0.11467*

*Language: Python*

1.Data tidying:
* replaced NA values with none,0,median or the most frequent values
* transform skewed data using boxcox transformation

2.Feature engineering:
 created feature ‘TotalSF’ as a combination of 'TotalBsmtSF','1stFlrSF' and '2ndFlrSF'
* created feature ‘TotBsmtFin’ as a combination of 'BsmtFinSF1' and 'BsmtFinSF2'
* created feature ‘TotBath’ as a combination ‘FullBath’,’HalfBath’,’BsmtFullBath’ and ‘BsmtHalfBath’

3.Feature selection:
* Keep only feature that have coefficients different than zero using LASSO model

4.Modelization:
* Ridge Model
* LASSO Model
* Extreme Gradient Boosting Model
* Gradient Boosting Model
* Light Gradient Boosting Model
* Single-Hidden Layer Perceptron Model (using Tensorflow with normalized features)

5.Training:
* Average of 5-folds cross validation (for the first five models)

6.Results:
* Weighted Average of the models above
