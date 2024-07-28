# Feature Scaling, Cost Function and Gradient Descent in MLR

![image](https://github.com/user-attachments/assets/4b5d71b1-f282-48a1-b1bc-7fbd606b20b4)


# Cost Function and Its Minimization

The cost function `J(θ)` is defined as follows:

$$
J(θ_0, θ_1, ..., θ_n) = \frac{1}{2m} \sum_{i=1}^{m} [h_θ(x^{(i)}) - y^{(i)}]^2
$$

Where:
- `m` is the number of training examples
- `x^{(i)}` and `y^{(i)}` are the input features and target variable for the ith training example respectively
- `h_θ(x)` is our hypothesis function defined by:

$$
h_θ(x) = θ_0 + θ_1x_1 + ... + θ_nx_n
$$

The main goal in machine learning regression problems is to minimize the value of `J(θ)`, which represents how well our hypothesis function fits the data.

For more information go to [03-Cost Function.md](https://github.com/ofcoursenp/CS229/blob/main/Lectures/03-Cost%20Function.md)

# Gradient Descent

![image](https://github.com/user-attachments/assets/0b6ef7dc-4fb4-4571-a6bc-3b634cde5583)


Gradient descent is an optimization algorithm used to minimize a cost function by iteratively moving towards the minimum value of the function. The update rule for the parameter `θ_j` is given by:

$$
\theta_j := \theta_j - \alpha \frac{\partial}{\partial \theta_j} J(\theta_0, \theta_1, ..., \theta_n)
$$

Where:
- `θ_j` is the parameter being updated
- `α` is the learning rate, which controls the step size of each update
- `J(θ_0, θ_1, ..., θ_n)` is the cost function

For example, if we use the mean squared error as the cost function, the update rule becomes:

$$
\theta_j := \theta_j - \alpha \frac{1}{m} \sum_{i=1}^{m} (h_\theta(x^{(i)}) - y^{(i)}) x_j^{(i)}
$$

Where:
- `m` is the number of training examples
- `h_θ(x)` is the hypothesis function
- `x_j^{(i)}` is the feature value of the j-th parameter for the i-th training example
- `y^{(i)}` is the actual output for the i-th training example

The main goal of gradient descent is to minimize the cost function `J(θ)` by updating the parameters `θ` in the direction that reduces the cost.

For more information go to [04-Gradient Descent.md](https://github.com/ofcoursenp/CS229/blob/main/Lectures/04-Gradient%20Descent.md)


# Feature Scaling

Feature scaling is a method used to normalize the range of independent variables or features of data. In data processing, it is also known as data normalization and is generally performed during the data preprocessing step. The goal of feature scaling is to ensure that all features contribute equally to the model's performance.

Feature scaling is important in algorithms that compute distances between data points, such as k-nearest neighbors (KNN) or clustering algorithms like k-means.

The following image illustrates the concept of feature scaling:

![image](https://github.com/user-attachments/assets/dc66dcaf-6afd-49ce-b0ee-4f09deafa949)

## Explanation

In the left plot, the features are on different scales, leading to elongated contours, indicating that one feature has a much larger range than the other. This can cause issues in machine learning algorithms that rely on distance measurements.

In the right plot, the features have been scaled to be on a similar range, resulting in circular contours. This shows that the features are now contributing equally, which helps improve the performance of many machine learning algorithms.

To make sure features are on a similar scale, various techniques such as normalization or standardization can be used.


# Mean Normalization

![image](https://github.com/user-attachments/assets/418759a9-4ff3-4f8a-8bad-484704011930)

## Mean Normalization

Mean normalization is a feature scaling technique used to standardize the range of independent variables or features of data. The formula for mean normalization is:

$$\[ x' = \frac{x - \text{(Avg of x)}}{\text{Max} - \text{Min}} \]$$

### Explanation

- $$\( x \)$$: The original value of the feature.
- $$\( \text{Avg of x} \)$$: The average (mean) value of the feature.
- $$\( \text{Max} \)$$: The maximum value of the feature.
- $$\( \text{Min} \)$$: The minimum value of the feature.
- $$\( x' \)$$: The normalized value of the feature.

The numerator $$\( x - \text{(Avg of x)} \)$$ represents the difference between a particular value of $$\( x \)$$ and the average value of $$\( x \)$$. The denominator $$\( \text{Max} - \text{Min} \)$$ represents the range of $$\( x \)$$, which is the difference between the maximum and minimum values of $$\( x \)$$.


