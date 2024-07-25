# What is Simple Linear Regression model


![image](https://github.com/user-attachments/assets/951d9f67-4d93-499f-8945-3e9f45bc0416)


# Simple Linear Regression

Simple Linear Regression is a statistical method that allows us to summarize and study relationships between two continuous (quantitative) variables. This method is termed as "simple" because it examines the relationship between two variables only.

## Formula Representation

The formula for a simple linear regression is:

$$ h_{\theta}(x) = \theta_0 + \theta_1 \cdot x_1 $$

- `h_{\theta}(x)` represents the predicted value of the dependent variable (DV) for any given value of the independent variable (IV).
- `θ_0` is the constant term; it's the value of `h_{\theta}(x)` when `x_1` is 0.
- `θ_1` represents the coefficient of the independent variable; it's the amount by which `h_{\theta}(x)` changes with a one-unit change in `x_1`.

## Components

- **Dependent Variable (DV):** This is what we are trying to predict or explain.
- **Independent Variable (IV):** This is what we are using to predict or explain the DV.
- **Constant:** Also known as the y-intercept in linear regression, it allows for a starting point for predicting DV.
- **Coefficient:** Indicates how much DV will change when IV changes.


![image](https://github.com/user-attachments/assets/9bb55856-f628-4817-877e-90c8afc27447)


# Salary Prediction Model

The following graph illustrates a linear regression model that predicts salary based on years of experience.

!Salary vs Experience Scatter Plot

## Model Explanation

- The scatter plot shows individual data points marked with red stars, each representing an individual's salary at their respective level of experience.
- A line of best fit is drawn through these data points, represented by the equation \( h_\theta(x) = \theta_0 + \theta_1 * x_1 \).
- The horizontal axis denotes years of experience.
- The vertical axis denotes salary in dollars, starting at 30k and increasing in increments of 10k.
- Parameters:
  - $$\( \theta_0 \)$$: Represents the starting salary without any experience (y-intercept).
  - $$\( \theta_1 \)$$: Represents the increase in salary for each additional year of experience (slope).

This model can be used to predict future salaries based on an individual's years of experience using machine learning techniques.




