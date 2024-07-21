# **Data Preprocessing**

![image](https://github.com/user-attachments/assets/da19b85e-3860-4a52-b637-baa458ae5dc5)

# **column normalization**

![image](https://github.com/user-attachments/assets/808c66c6-c306-4053-96f7-aed89bbb01c3)

**Column Headers:**

* The first column is labeled “Player,” with entries ranging from “Player 1” to “Player 9.”

* The second column is labeled “Height (inches),” and the values range from 69 to 76 inches.

* The third column is labeled “Weight (pounds),” and the values range from 180 to 235 pounds.


**Normalization Formula:**

To the right of the table, there’s a mathematical formula inside a black rectangle: $$[ A_i = \frac{A_i - A_{\text{min}}}{A_{\text{max}} - A_{\text{min}}} ]$$

Here, ( A_i ) represents an individual value (either height or weight).

( $$A_{\text{min}}$$ ) represents the minimum value in the dataset (e.g., minimum height or weight).
( $$A_{\text{max}}$$ ) represents the maximum value in the dataset (e.g., maximum height or weight).

**Purpose:**

* This formula is used for normalizing data within a specific range (usually between 0 and 1). Normalization is common in statistical analysis and machine learning tasks.

# **Column Standardization**

![image](https://github.com/user-attachments/assets/4e27130f-638e-445e-8012-16d89d3f9678)

**Scaling by Standard Deviation:**

Divide each mean-centered value by the standard deviation of the feature.

This scales the data to have a standard deviation of 1.

Mathematically, the standardized value Ai​ becomes : $$A_i = \frac{A - \overline{A}}{\text{Std}}$$

where Std represents the standard deviation of feature A.

# **Left one is after Column Standardization and Right one is before Column Standardization**

![image](https://github.com/user-attachments/assets/dba5e934-4c62-4d0c-8cc6-a1a776b0d4e7)
