# Linear Regression

Linear Regression is a supervised leanring algorithm used for predictive analysis. It models the relationship between two variables by fitting a linear equation to the observed data. One variable is considered the independent variable (features), and the other is the dependent variable (output or target).

The general form of the linear equation is:

<p align="center">
$y = b_{0} + b_{1}x$
</p>

Where:
- $y$ is the predicted output
- $x$ is the input features(s)
- $b_{0}$ is the intercept (the value of $y$ when $x=0$)
- $b_{1}$ is the slop (the change in $y$ when $x$ increases by 1 unit)

The goal is to find the best-fit line by minimizing the residual sum of squares between the observed targets in the dataset and the targets predicted by the linear approximation

# Multiple Linear Regression

Multiple Linear Regression is an extension of simple linear regression and involves more than one inependent variable (or feature) to predict the dependent variable (target). The goal is the same as simple linear regression: to fit a line (or plane, or hyperplane) that best explains the relationship between the input features and the output target.

The general form of the multiple linear regression equation is:

<p align="center">
$y = b_{0} + b_{1}x_{1}  + b_{2}x_{2} + ... + b_{n}x_{n}$
</p>

Where:
- $y$ is the predicted output
- $x_{1},x_{2},...$ are the independent variables
- $b_{0}$ is the intercept
- $b_{1}, b_{2},...$ are the coefficients for each feature (how much each feature contributes to the output)


# $R^{2}$ (R-Squared) Error

It is a statistical measure that repersents the proportion of the variance in the dependent variable (target) that is predictable from the independent variables (features). It essentially indicates how well the regession model fits the data.

The fomula is:

<p align="center">
$R^{2} = 1 - \frac{SS_{res}}{SS_{tot}}$
</p>

Where:
- $SS_{res}$ is the sum of squared residuals (known as the sum of squared errors), which is the different between the actual and predicted values.
- $SS_{tot}$ is the total sum of squares, which is the difference between the actual values and the mean of the actual values.

## Interpretation of $R^{2}$
- $R^{2} = 1$ Perfect fit. The model explains 100% of the variance in the target variable
- $R^{2} = 0$ The model explains non of the variance, it's no better than simply prediting the mean of the target
- $R^{2} < 0$ The model is worse than predicting the mean value of the target. This usually happens when the moel is poorly fitted or when you're dealing with overfitting in training data bet no in test data

## Intuition 
- High $R^{2}$: Implies the model does a good job explaining the variablility in the data
- Low $R^{2}$: Implies the moel does not capture the unerlying pattern in the data well. The features used might not be sufficient or informative enough to explain the target
