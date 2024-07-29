# SVR

![image](https://github.com/user-attachments/assets/d752830e-90da-4f8b-a932-50f446c15a1a)

![image](https://github.com/user-attachments/assets/b64376e0-4531-4420-b91a-d2fe56114cae)

# Support Vector Regression (SVR)

Support Vector Regression (SVR) is a type of Support Vector Machine (SVM) used for regression tasks. While SVMs are typically used for classification, SVR adapts the concept to predict continuous values.

## Key Concepts

1. **Margin of Tolerance (Epsilon)**: SVR attempts to fit the error within a specified margin of tolerance, denoted by `ε` (epsilon). The idea is to ensure that errors within this margin are not penalized.

2. **Hyperplane**: In the context of SVR, the hyperplane is the line that fits the data best according to the specified margin. The goal is to find the hyperplane that maximizes the margin while minimizing the prediction error.

3. **Support Vectors**: These are the data points that lie on the boundaries of the margin. They are crucial for defining the position of the hyperplane. In SVR, support vectors are the points that are within or on the boundary of the epsilon margin.

## How SVR Works

1. **Define the Margin**: Set the margin of tolerance `ε` around the hyperplane. This is the region where errors are not penalized.
   
2. **Fit the Hyperplane**: Find the hyperplane that best fits the data while ensuring that the majority of the data points lie within the margin of tolerance.
   
3. **Minimize the Error**: Penalize data points that fall outside the epsilon margin. The objective is to find the hyperplane that minimizes this penalization.

4. **Optimization**: Solve the optimization problem that aims to minimize the norm of the weights (for simplicity) and the error penalties.

## Mathematical Formulation

The objective function for SVR can be expressed as:

$$\[ \min \frac{1}{2} ||w||^2 + C \sum_{i=1}^n (\xi_i + \xi_i^*) \]$$

Where:
- $$\( w \)$$ is the weight vector.
- $$\( C \)$$ is a regularization parameter that controls the trade-off between the flatness of the hyperplane and the amount up to which deviations larger than \( \epsilon \) are tolerated.
- $$\( \xi_i \)$$ and $$\( \xi_i^* \)$$ are slack variables that measure the degree of deviation from the margin.

Subject to:
$$\[ y_i - \langle w, x_i \rangle - b \leq \epsilon + \xi_i \]$$
$$\[ \langle w, x_i \rangle + b - y_i \leq \epsilon + \xi_i^* \]$$
$$\[ \xi_i, \xi_i^* \geq 0 \]$$

Where:
- $$\( \langle w, x_i \rangle + b \)$$ represents the predicted value.
- $$\( y_i \)$$ is the actual value.

## Example Plot

Below is a graphical representation of SVR:

![image](https://github.com/user-attachments/assets/76841012-c46b-45d7-8dc3-8322ab45c279)


In the graph:
- The black line represents the hyperplane.
- The green lines represent the boundaries of the margin of tolerance (epsilon).
- The blue points within the green lines are the support vectors.
- The red points outside the green lines are the outliers or points penalized for falling outside the epsilon margin.

## Conclusion

Support Vector Regression is a powerful tool for regression analysis, especially when you need a model that can handle a certain margin of error effectively. By maximizing the margin and minimizing the error penalties, SVR provides a robust method for predicting continuous values.

