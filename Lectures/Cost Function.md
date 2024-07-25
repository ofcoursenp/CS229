# What is Cost Function


![image](https://github.com/user-attachments/assets/6942610a-ba98-454f-b466-78850402b151)

**Axes and Labels:**

* The x-axis represents “Experience,” which likely corresponds to the number of years of experience.

* The y-axis represents “Salary ($),” indicating the salary amount.

* The labels help us understand what each axis represents.

**Data Points:**

* The red stars on the graph represent individual data points. Each point corresponds to a specific combination of experience and salary.

* These data points are scattered across the graph.

**Linear Regression Model**

The green dashed line represents a linear regression model. This model attempts to predict salary based on experience.
The equation associated with the model is: hθ​(x)=θ0​+θ1​⋅x1​


Here, (h_θ(x)) is the hypothesis function.

(θ_0) and (θ_1) are the model parameters (intercept and coefficient).

(x_1) represents the experience (input feature).

**Annotations:**

* The “+10K” annotation on the y-axis indicates an increment of $10,000 in salary.

* The “+1 Year” annotation on the x-axis represents a one-year increase in experience.


### Overview
![image](https://github.com/user-attachments/assets/78f347ee-b856-4337-970c-b3451003a088)


This scatter plot graph illustrates the relationship between salary and work experience. We'll explore the key components of the graph and the underlying linear regression model.

### Graph Elements

1. **Axes and Labels:**
   - **X-Axis:** Represents "Experience" (years of work experience).
   - **Y-Axis:** Represents "Salary ($)".

2. **Data Points:**
   - Red star-shaped data points represent individual observations.
   - Each point corresponds to a specific combination of experience and salary.

3. **Linear Regression Model:**
   - The blue line represents the best-fit line (trend line).
   - Equation: $$ h_θ(x) = θ_0 + θ_1 \cdot x_1 $$
     - \(h_θ(x)\): Hypothesis function.
     - \(θ_0\), \(θ_1\): Model parameters (intercept and coefficient).
     - \(x_1\): Experience (input feature).

4. **Residuals:**
   - Dashed lines connect data points to the trend line.
   - These represent residuals (differences between actual and predicted salaries).

5. **Objective:**
   - Minimize the sum of squared residuals: $$ \sum (y - \hat{y})^2 $$
   - This ensures the best-fitting line.


## Cost Function and Mean Square Error Method

![image](https://github.com/user-attachments/assets/3d50b0e5-59a9-4a9e-ae13-0421d7a9b493)


The image presents a mathematical representation of a cost function used in machine learning, specifically for linear regression. The cost function \(J(θ₀, θ₁)\) is defined as one half of the mean of the sum of squared differences between predicted values \(hθ(x⁽ⁱ⁾)\) and actual values \(y⁽ⁱ⁾\). This is mathematically represented as:

$$\[ J(θ₀, θ₁) = \frac{1}{2m} \sum_{i=1}^{m} (hθ(x⁽ⁱ⁾) - y⁽ⁱ⁾)^2 \]$$

Where:
- \(m\) is the number of training examples,
- \(hθ(x)\) is the hypothesis function, defined as \(θ₀ + θ₁xᵢ\),
- \((x⁽ⁱ⁾, y⁽ⁱ⁾)\) are the training examples.

The main goal in this context is to minimize the value of parameters \(θ₀\) and \(θ₁\), which is achieved through an optimization algorithm. The method used for minimization in this scenario is referred to as the Mean Square Error Method.

