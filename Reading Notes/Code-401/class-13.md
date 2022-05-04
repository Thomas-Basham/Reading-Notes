# Class 13
## Reading
### [How to Run Linear Regression in Python](http://bigdata-madesimple.com/how-to-run-linear-regression-in-python-scikit-learn/)
- The overall idea of regression is to examine two things: 
  - (1) does a set of predictor variables do a good job in predicting an outcome (dependent) variable?  
  - (2) Which variables in particular are significant predictors of the outcome variable, and in what way do they–indicated by the magnitude and sign of the beta estimates–impact the outcome variable? 
- Scikit-learn is a powerful Python module for machine learning
- from sklearn.linear_model import LinearRegression
- lm.fit() -> fits a linear model
- lm.predict() -> Predict Y using the linear model with estimated coefficients
- lm.score() -> Returns the coefficient of determination (R^2). A measure of how well observed outcomes are replicated by the model, as the proportion of total variation of outcomes explained by the model.
- In practice, you won't implement linear regression on the entire data set, you will have to split the data sets into training and test data sets.
## Additional Resources
### [Linear Regression in Python](https://realpython.com/linear-regression-in-python/)
## Videos

### [Introduction to Simple Linear Regressions](https://www.youtube.com/watch?v=KsVBBJRb9TE)

## Bookmark and Review

### [Train & Test Splits](https://towardsdatascience.com/train-test-split-and-cross-validation-in-python-80b61beca4b6)

### [What is Linear Regression](https://www.statisticssolutions.com/what-is-linear-regression/)
