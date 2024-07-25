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


**Converting it into 2-D form , plotting a graph of θ1 and θ2**

![image](https://github.com/user-attachments/assets/3890253a-93a6-4ebb-b646-294c8e02afe8)


