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
  
