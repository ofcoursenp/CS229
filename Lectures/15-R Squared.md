# R-squared and Adjusted R-squared in R for Machine Learning

## Introduction
R-squared and Adjusted R-squared are statistical measures used to evaluate the goodness of fit for regression models. While R-squared measures the proportion of the variance for a dependent variable that's explained by an independent variable or variables, Adjusted R-squared adjusts for the number of predictors in the model, providing a more accurate measure.

## Formulas
The formulas for R-squared and Adjusted R-squared are:

### R-squared
$$
R^2 = 1 - \frac{SS_{res}}{SS_{tot}}
$$

### Adjusted R-squared
$$
\bar{R}^2 = 1 - \left( \frac{(1 - R^2)(n - 1)}{n - k - 1} \right)
$$

Where:
- \( SS_{res} \) is the sum of squares of the residual errors.
- \( SS_{tot} \) is the total sum of squares.
- \( n \) is the number of observations.
- \( k \) is the number of predictors.

## Calculation in R
Here's how you can calculate R-squared and Adjusted R-squared in R:

```r
# Sample data
observed <- c(1, 2, 3, 4, 5)
predicted <- c(1.1, 1.9, 3.2, 3.8, 5.1)

# Calculate the mean of observed values
mean_observed <- mean(observed)

# Calculate the total sum of squares (SStot)
SStot <- sum((observed - mean_observed)^2)

# Calculate the residual sum of squares (SSres)
SSres <- sum((observed - predicted)^2)

# Calculate R-squared
R_squared <- 1 - (SSres / SStot)

# Number of observations
n <- length(observed)

# Number of predictors (for simplicity, assuming 1 predictor)
k <- 1

# Calculate Adjusted R-squared
Adjusted_R_squared <- 1 - ((1 - R_squared) * (n - 1) / (n - k - 1))

# Print R-squared and Adjusted R-squared
print(paste("R-squared:", R_squared))
print(paste("Adjusted R-squared:", Adjusted_R_squared))
