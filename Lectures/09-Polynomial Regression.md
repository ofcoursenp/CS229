# Polynomial Regression


![image](https://github.com/user-attachments/assets/37234027-d1f5-4b42-a0b3-dad47e4447e3)

## Polynomial Regression
The equation for polynomial regression is:
$$\[ h_\theta(x)$$ = $$\theta_0 + \theta_1 x + \theta_2 x^2 + \ldots + \theta_n x^n \]$$
- $$\( h_\theta(x) \)$$: Predicted value
- $$\( \theta_0 \)$$: Intercept
- $$\( \theta_1, \theta_2, \ldots, \theta_n \)$$: Coefficients for the polynomial terms
- $$\( x, x^2, \ldots, x^n \)$$: Polynomial terms of the independent variable

# Polynomial Regression

Polynomial regression is a type of regression analysis where the relationship between the independent variable \( x \) and the dependent variable \( y \) is modeled as an \( n \)-th degree polynomial. This allows for a more flexible fit to the data compared to simple linear regression, which assumes a straight-line relationship.

## Key Points of Polynomial Regression

1. **Equation**:
   The general form of a polynomial regression model is:
   $$\[ h_\theta(x) = \theta_0 + \theta_1 x + \theta_2 x^2 + \ldots + \theta_n x^n \]$$
   Here, $$\( \theta_0, \theta_1, \ldots, \theta_n \)$$ are the coefficients of the polynomial, and $$\( x, x^2, \ldots, x^n \)$$ are the polynomial terms of the independent variable.

2. **Nonlinear Relationship**:
   Polynomial regression can capture the nonlinear relationship between the independent variable and the dependent variable. For example, if the data shows a curved trend, a polynomial regression can fit this curve better than a linear regression.

3. **Degree of the Polynomial**:
   The degree $$\( n \)$$ of the polynomial determines the flexibility of the model. A higher degree polynomial can fit more complex patterns in the data, but it also increases the risk of overfitting, where the model fits the noise in the data rather than the underlying trend.

4. **Linear in Parameters**:
   Despite fitting a nonlinear relationship, polynomial regression is considered linear in terms of the parameters $$\( \theta \)$$. This means that the estimation of the coefficients can be done using linear regression techniques.

## Example
Suppose we have data points that form a parabolic shape. A simple linear regression might not fit the data well, but a polynomial regression with a degree of 2 (quadratic) can model the parabolic relationship effectively:
$$\[ y = \theta_0 + \theta_1 x + \theta_2 x^2 \]$$

## Applications
Polynomial regression is used in various fields such as economics, biology, and engineering to model complex relationships between variables. It's particularly useful when the relationship between the variables is not strictly linear.

# Difference

![image](https://github.com/user-attachments/assets/de89ceb3-7a0b-4517-a348-e16a329aecdd)

![image](https://github.com/user-attachments/assets/c6a5ca6f-17db-4d71-9fd0-191f5e2c6b41)


# Cost function and Gradient Descent

![image](https://github.com/user-attachments/assets/70c79f06-3b0a-4db9-9b36-a3b898a418e7)

For more info on Gradient Descent and Cost function watch the Lecture [03-Cost function](https://github.com/ofcoursenp/CS229/blob/main/Lectures/03-Cost%20Function.md) and [04-Gradient Descent](https://github.com/ofcoursenp/CS229/blob/main/Lectures/04-Gradient%20Descent.md)
