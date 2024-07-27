# Gradient Descent

![image](https://github.com/user-attachments/assets/2c00aa30-d6e2-4cba-9597-fb5b9c2ae5c1)

![image](https://github.com/user-attachments/assets/414c4492-1f54-4093-bb6a-a2e8adbba693)

![image](https://github.com/user-attachments/assets/ab5e3015-892c-4190-8464-13bfb4fe8cd2)

# Gradient Descent: An Overview

Gradient Descent is an iterative optimization algorithm used to minimize a given function (often referred to as the **cost function** or **loss function**). It's widely employed in machine learning for tasks like training neural networks, linear regression, and logistic regression. Here are the key points:

1. **Objective**: The primary goal of Gradient Descent is to find the minimum value of a cost function by adjusting the model parameters (also known as weights or coefficients).

2. **Algorithm Steps**:
   - Initialize the model parameters randomly (e.g., θ0, θ1, etc.).
   - Compute the gradient (partial derivatives) of the cost function with respect to each parameter.
   - Update the parameters using the gradient information:
     ```
     θ_i = θ_i - α * ∂J(θ) / ∂θ_i
     ```
     where:
     - $$\(J(θ)\)$$ is the cost function.
     - $$\(\alpha\)$$ (learning rate) controls the step size in each iteration.
   - Repeat the above steps until convergence (i.e., the cost function reaches a minimum or a predefined number of iterations is reached).

3. **Intuition**: Imagine standing on a hilly terrain (the cost function surface). Your goal is to reach the lowest point (minimum cost). Gradient Descent guides you by indicating the steepest downhill direction, allowing you to take steps toward the valley.

4. **Types of Gradient Descent**:
   - **Batch Gradient Descent**: Computes gradients using the entire dataset.
   - **Stochastic Gradient Descent (SGD)**: Computes gradients using a single random data point.
   - **Mini-Batch Gradient Descent**: Computes gradients using a small subset (mini-batch) of the data.

5. **Hyperparameters**:
   - **Learning Rate (\(\alpha\))**: Determines the step size. Too large, and you might overshoot the minimum; too small, and convergence is slow.
   - **Number of Iterations**: Decide how many times to update the parameters.

## Visualizing Gradient Descent

The image you provided illustrates this concept visually. The multicolored surface represents the cost function \(J(θ)\) with respect to two parameters (\(θ_0\) and \(θ_1\)). The green stars trace the path taken by Gradient Descent as it iteratively adjusts the parameters to minimize the cost function.


# Local and global minimum

![image](https://github.com/user-attachments/assets/3d2a05a9-8bc7-4500-b7f5-cff7e25fd77b)

**For more info about minima and maxima click here ---> <a href="https://github.com/ofcoursenp/CS229/blob/main/Mathematics/Calculus/Lecture_3.md">Lecture 3 - Calculus</a>**

# Visualising

![image](https://github.com/user-attachments/assets/f9a31305-23e4-4371-8640-57d12a79e16a)


#**Converting it into 2-D form , plotting a graph of θ1 and θ2**

![image](https://github.com/user-attachments/assets/3890253a-93a6-4ebb-b646-294c8e02afe8)

#**Going inside the Deep point of the graph**

![image](https://github.com/user-attachments/assets/9435f3ed-b050-4b28-a499-519b67520ef1)

## Gradient Descent Update Rule

The gradient descent update rule for parameter θ_j is given by:

$$
\theta_j := \theta_j - \alpha \frac{\partial}{\partial \theta_j} J(\theta_0, \theta_1)
$$

Where:
- **θ_j**: Parameter being updated
- **α**: Learning rate
- **∂/∂θ_j**: Partial derivative with respect to θ_j
- **J(θ_0, θ_1)**: Cost function


#How learning rate effects on gradient descent
![image](https://github.com/user-attachments/assets/d41fd5ce-25b6-4720-8887-2c223fb91e22)

## Learning Rate Illustration

!Learning Rate Illustration

### Left Graph: When Learning Rate is too Small
- Shows a green U-shaped curve with red dots closely following along, indicating slow convergence.

### Right Graph: When Learning Rate is too Large
- Displays a similar green U-shaped curve with red dots scattered widely, suggesting inefficient convergence due to overly large steps.

# How to know where to move?
![image](https://github.com/user-attachments/assets/ec6f5b36-3603-4faf-90e3-3e17f24e0848)

## Optimization Graphs

### Left Graph
- **Equation:** $$\theta_j = \theta_i - \alpha a \text{ (Positive Number)}$$
- Demonstrates how subtracting a positive number (αa) from an initial value (θi) results in moving left along 'θ1'.

### Right Graph
- **Equation:** $$\theta_j = \theta_i - \alpha a \text{ (Negative Number)}$$
- Shows how subtracting a negative number (αa) from an initial value (θi) results in moving right along 'θ1'.

# Final understanding

## Gradient Descent and Derivatives

In gradient descent, the derivative of the cost function is crucial for updating the model's parameters. Here's a brief overview:

1. **Cost Function**: Measures the error between predicted and actual values.
2. **Derivative (Gradient)**: Indicates the slope of the cost function, guiding the direction of parameter updates.
3. **Update Rule**: Parameters are updated to minimize the cost function.

### Steps:
1. **Calculate the Gradient**: Compute the derivative of the cost function with respect to each parameter.
2. **Update Parameters**: Adjust the parameters using the formula:

$$
\theta_j := \theta_j - \alpha \frac{\partial}{\partial \theta_j} J(\theta)
$$

Where:
- **θ_j**: Parameter being updated
- **α**: Learning rate
- **∂/∂θ_j**: Partial derivative with respect to θ_j
- **J(θ)**: Cost function

**Note : No need for mathematic calculations for now because all the calculations is done by computer itself**

