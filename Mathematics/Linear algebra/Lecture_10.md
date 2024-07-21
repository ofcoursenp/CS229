# **Please watch these videos before going on toward the note It will provide better understanding <a href="https://www.youtube.com/playlist?list=PL09TaaZh44U0KnzGPbQN1MLrznJg-5No_">Click Here</a>**

# **Dimensionality Reduction**

![image](https://github.com/user-attachments/assets/c5be2a2b-d56a-4346-a1ce-4c3e3af1aeec)

**What is PCA?**

PCA is a dimensionality reduction technique commonly used in data science and machine learning. Its primary goal is to transform high-dimensional data into a lower-dimensional space while preserving as much variance as possible. Here’s how it works:


**Data Preparation:**

* Suppose we have a dataset with multiple features (dimensions). For example, imagine a dataset containing information about houses, including features like square footage, number of bedrooms, and price.

* Each house corresponds to a data point in this high-dimensional space.

**Centering the Data**

* We start by centering the data. This means subtracting the mean of each feature from all data points. Centering ensures that the transformed data has zero mean.

**Covariance Matrix Calculation:**

* Next, we compute the covariance matrix for the centered data. The covariance between two features indicates how they vary together.

* The diagonal elements of the covariance matrix represent the variance of each feature.

**Eigenvalue Decomposition:**

* We find the eigenvectors and eigenvalues of the covariance matrix.

* Eigenvectors represent the directions of maximum variance (principal components), and eigenvalues quantify the amount of variance along these directions.

**Selecting Principal Components:**

* We sort the eigenvalues in descending order. The eigenvectors corresponding to the largest eigenvalues are our principal components.
  
* These principal components form a new coordinate system for our data.

**Projecting Data onto Principal Components:**

* Finally, we project our original data points onto the principal components.
 
* The first principal component captures the most variance, the second captures the second most, and so on.
