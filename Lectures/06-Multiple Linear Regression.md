# Multiple Linear Regression

![image](https://github.com/user-attachments/assets/de1efa35-c1cb-40b1-9166-7861592f77fd)

# Linear Regression Formulas

## Simple Linear Regression
$$h_\theta(x) = \theta_0 + \theta_1 \cdot x_1$$

## Multiple Linear Regression
$$h_\theta(x) = \theta_0 + \theta_1 \cdot x_1 + \theta_2 \cdot x_2 + \ldots + \theta_n \cdot x_n$$

#

![image](https://github.com/user-attachments/assets/393f2f54-e85e-4834-a534-f0db3a66ae1b)

## Multiple Linear Regression with Categorical Data

The table below shows a dataset containing several features (`R&D Spend`, `Admin`, `Marketing`, `State`) and an output (`Profit`). The `State` feature is a categorical variable, which has been encoded using one-hot encoding to create two new binary features: `New York` and `California`.

| Profit   | R&D Spend | Admin   | Marketing | State      | New York | California |
|----------|-----------|---------|-----------|------------|----------|------------|
| 191,261.8| 152,987.9 | 166,993 | 471,098   | New York   | 1        | 0          |
| 182,987.9| 166,993.1 | 191,874 | 678,232   | California | 0        | 1          |
| 196,993.1| 131,261.8 | 198,874 | 643,981   | California | 0        | 1          |
| 182,298.0| 152,298.0 | 131,261 | 246,941   | New York   | 1        | 0          |
| 201,874.6| 191,874.6 | 142,789 | 973,756   | California | 0        | 1          |

### One-Hot Encoding

To include the categorical `State` feature in the regression model, one-hot encoding is used. This converts the `State` variable into two binary variables:
- `New York`: A binary variable that is 1 if the state is New York, otherwise 0.
- `California`: A binary variable that is 1 if the state is California, otherwise 0.

Note: Typically, one-hot encoding includes a variable for each category minus one to avoid the dummy variable trap. However, in this example, it seems both binary variables are included for clarity.

### Regression Equation

The multiple linear regression equation is given as:

$$\[ h_\theta(x) = \theta_0 + \theta_1 \cdot x_1 + \theta_2 \cdot x_2 + \theta_3 \cdot x_3 \]$$

Where:
- $$\( h_\theta(x) \)$$: Predicted Profit
- $$\( \theta_0 \)$$: Intercept term
- $$\( \theta_1 \)$$: Coefficient for `R&D Spend`
- $$\( \theta_2 \)$$: Coefficient for `Admin`
- $$\( \theta_3 \)$$: Coefficient for `Marketing`
- $$\( x_1, x_2, x_3 \)$$: Independent variables

#

![image](https://github.com/user-attachments/assets/7926f75f-76aa-40fc-a435-ebce934ae942)

![image](https://github.com/user-attachments/assets/787be74d-d9a3-4b35-95dc-5ef7d20cb08c)

**A dummy variable (also known as indicator variable or just dummy) is one that takes a binary value (0 or 1) to indicate the absence or presence of some categorical effect that may be expected to shift the outcome**
**In this case we dont need California column so we removed that column**

# Feature Selection

![image](https://github.com/user-attachments/assets/381f0fd4-cfa7-4b8f-8e48-5b30ef9563f2)

**Feature selection is the process of isolating the most consistent, non-redundant, and relevant features to use in model construction. Methodically reducing the size of datasets is important as the size and variety of datasets continue to grow.**

![image](https://github.com/user-attachments/assets/1b8ae8a9-dfb4-4f2f-846d-ceea87f76152)

# Building a model
![image](https://github.com/user-attachments/assets/447ab361-bf3b-403f-8f9c-dec55d3276e8)

# Backward Elimination

![image](https://github.com/user-attachments/assets/a35e941b-efa8-4bc6-912e-de6d58fb3b10)

## Backward Elimination

Backward Elimination is a step-by-step process used in statistical models to select significant variables. Here's how it works:

1. **Step 1:** Select a significance level to stay in the model (e.g., SL = 0.05).
2. **Step 2:** Fit the full model with all possible predictors.
3. **Step 3:** Consider the predictor with the highest P-value. If P > SL, proceed to Step 4; otherwise, go to FINISH.
4. **Step 4:** Remove the predictor with the highest P-value.
5. **Step 5:** Fit the model without this variable and go back to Step 3.

This iterative process continues until no predictor has a P-value higher than the significance level, resulting in a model that includes only statistically significant variables.

![image](https://github.com/user-attachments/assets/53064b2c-4de1-48db-bb50-4bbff728a516)

# Backward Elimination Process

Backward Elimination is a step-by-step method used in statistical models for selecting only significant variables. The steps are as follows:

1. **Select a significance level** to stay in the model (e.g., SL = 0.05).
2. **Fit the full model** with all possible predictors.
3. **Consider the predictor** with the highest p-value. If P > SL, go to step 4; otherwise, go to FIN.
4. **Remove the predictor** with the highest p-value.
5. **Fit the model** without this variable and go back to step 3.
6. **FIN:** Your model is ready.

This method ensures that only statistically significant features are included in your final model.


# Forward Selection

![image](https://github.com/user-attachments/assets/c8c57696-82c1-4079-8eb5-919d5c07d74b)

# Forward Selection Process

Forward Selection is a step-by-step method used in statistical models for selecting significant variables. The steps are as follows:

1. **Select a significance level** to stay in the model (e.g., SL = 0.05).
2. **Fit all simple regression models**. Select the one with the lowest P-value.
3. **Keep the variable** and fit all possible models with one extra predictor added to the ones you already have.
4. **Consider the predictor** with the lowest P-value. If P > SL, go back to step 3; otherwise, go to FIN.
5. **FIN:** Your model is ready.

This method ensures that only statistically significant features are included in your final model.


![image](https://github.com/user-attachments/assets/d66689fa-43bf-46ff-8efc-bb96afa5910d)

# Bidirectional Elimination

![image](https://github.com/user-attachments/assets/daba4b42-1371-401a-a0f6-890080a7febe)

# Bidirectional Elimination Process

Bidirectional Elimination is a statistical method used for model selection in regression analysis. It combines both forward selection and backward elimination to iteratively add and remove predictors based on their significance levels.

## Steps Involved:

1. **Initial Selection**: Choose significance levels for entering and staying in the model.
   - `SLENTER`: Significance level to enter (e.g., 0.05)
   - `SLSTAY`: Significance level to stay (e.g., 0.05)

2. **Forward Selection**: Add predictors that meet the entry significance level (`P < SLENTER`).

3. **Backward Elimination**: Remove predictors that do not meet the stay significance level (`P > SLSTAY`).

4. **Termination**: Repeat steps 2 and 3 until no new predictors can enter, and no existing predictors can exit.

