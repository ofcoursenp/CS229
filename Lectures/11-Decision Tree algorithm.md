# Decision Tree algorithm

![image](https://github.com/user-attachments/assets/133bfe09-198d-4c90-a809-795ecb7f1d23)

**Decision Tree algorithm is also known as CART algorithm because it can do classification and regression problem both**
#

![image](https://github.com/user-attachments/assets/e249e01d-9e3b-4817-a361-5004671fb240)


# Decision Tree Intuition

The image presents a scatter plot with the title "Decision Tree Intuition" at the top. The scatter plot is used to illustrate how a decision tree algorithm might categorize data points. 

- The x-axis is labeled as `X1` and ranges from 0 to beyond 40.
- The y-axis is labeled as `X2` and ranges from approximately 150 to above 200.
- There are numerous blue cross-shaped data points spread across the plot.
- Four green rectangles represent decision boundaries, with numerical values inside each rectangle are the mean of the boundaries of data:
    - Top left rectangle contains the value `65.7`.
    - Top right rectangle contains the value `1023`.
    - Bottom left rectangle contains the value `300.5`.
    - Bottom right rectangle contains the value `-64.1` and another small green rectangle within it containing the value `0.7`.

This visualization is relevant as it provides an intuitive understanding of how decision trees can be used in machine learning to split data into different categories based on certain threshold values along different features (in this case, X1 and X2).


# Goal : To find out where does the red cross in the 2-D graph lies

![image](https://github.com/user-attachments/assets/ab1b8b3a-be13-4d20-a717-6ad0252c0b16)

![image](https://github.com/user-attachments/assets/927cc6bc-260d-4b28-9617-d30a92b0e90b)

# Decision Tree Diagram

The image shows a decision tree diagram with binary splits based on conditions involving two variables, X1 and X2. Here's a breakdown of the tree structure:

1. **Root Node**:
    - **Condition**: X1 < 20
  
    - **Yes Branch**:
        - **Condition**: X2 < 200
            - **Yes Branch**: Terminal Node with value `300.5`
            - **No Branch**: Terminal Node with value `65.7`
    - **No Branch**:
        - **Condition**: X2 < 170
            - **Yes Branch**:
                - **Condition**: X1 < 40
                    - **Yes Branch**: Terminal Node with value `-64.1`
                    - **No Branch**: Terminal Node with value `0.7`
            - **No Branch**: Terminal Node with value `1023`

**Since our X1 is greater than 20 So our brance goes towards **No branch** , Now our X2 value is greater than 170 So our brance goes towards **No branch**, Finally our data is present at 1023 boundary Since 1023 is the final direction and leaf** 

This decision tree represents a model used for making predictions or decisions based on input variables through a series of binary choices. Each node represents a condition on a variable, and the branches represent the outcomes of these conditions, leading to either further conditions or terminal nodes with specific values.

