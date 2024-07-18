# **Dot Product, Matrix Multiplication, Matrix Addition**

# **Matrix addition**

![image](https://github.com/user-attachments/assets/65001586-b67f-407f-b16d-0b7b82dde719)

# **Equations:** 
There are two sets of equations.

Each set defines three variables: A, B, and C.

In both sets, A is a list of five elements: (a_1, a_2, a_3, a_4,) and (a_5).

B is also a list of elements: in the first set, there are five elements (b_1) to (b_5); in the second set, there are only four elements (b_1) to (b_4).
C is the result of element-wise addition of lists A and B.

# **Element-Wise Addition:**

In the first set: [C = [a_1 + b_1, a_2 + b_2, a_3 + b_3, a_4 + b_4, a_5 + b_5]]

In the second set: [C = [a_1 + b_1, a_2 + b_2, a_3 + b_3, a_4 + b_4]]

However, In the second set C the elements are uneven so the matrix addition cant occur 

#

![image](https://github.com/user-attachments/assets/2869bb77-7f40-42a0-90ea-31f1c58ac783)

**Matrix addition is a fundamental operation in linear algebra. When you add two matrices, they must have the same dimensions (i.e., the same number of rows and columns). The resulting matrix will have the same dimensions as the original matrices, and each corresponding element in the result is obtained by adding the corresponding elements from the input matrices.
Here’s how it works:**

Suppose we have two matrices:

![image](https://github.com/user-attachments/assets/b1487104-234a-408a-a283-fced55cfe617)

![image](https://github.com/user-attachments/assets/324f0523-9ca8-42d8-821d-ecf595ac2cec)


We can add them element-wise to get the result matrix:

![image](https://github.com/user-attachments/assets/91f91d8d-6304-468e-8714-019f6c0933d0)


So, the sum of matrices (A) and (B) is:

![image](https://github.com/user-attachments/assets/3307df89-2add-4545-9db4-7405e49d4959)


Remember that matrix addition is commutative, which means that (A + B) is the same as (B + A).

# **matrix subtraction**

![image](https://github.com/user-attachments/assets/d9a58408-f2ee-40e8-8153-72483bc87d70)


# **Dot Product**

![image](https://github.com/user-attachments/assets/171d7e31-bef7-41ba-8cbb-b098de8e701e)

# **Vectors A and B:**
Vector A is a horizontal vector with elements (a_1, a_2, a_3, \ldots, a_n).

Vector B is a vertical vector with elements (b_1, b_2, b_3, \ldots, b_n).

# **Dot Product Calculation:**

The dot product (also known as the inner product) is the sum of the products of corresponding elements from vectors A and B: [ C = a_1b_1 + a_2b_2 + \ldots + a_nb_n ]
Result:

The result of the dot product is a single scalar value, denoted as C.

The dimensions of vector A are indicated as ((1, n)), and for vector B as ((n, 1)), resulting in the dimension of C as ((1, 1)).

# **Matrix Multipication**

![image](https://github.com/user-attachments/assets/e6b7d7fb-2a9e-4474-93a5-4df3ab5c2e47)

![image](https://github.com/user-attachments/assets/6c093f87-acca-4657-9b84-5bb11a8022a5)

**Matrix multiplication is a fundamental operation in linear algebra. When you multiply two matrices, the resulting matrix is formed by taking dot products of rows from the first matrix with columns from the second matrix. Here’s how it works:**

# **Given two matrices:**

![image](https://github.com/user-attachments/assets/899286c9-2616-485b-9a43-4f6ed2bf3d47)


The resulting matrix, denoted as (C), is calculated as follows:

C=A⋅B

where each element (c_{ij}) in matrix (C) is obtained by multiplying the (i)th row of matrix (A) with the (j)th column of matrix (B):

![image](https://github.com/user-attachments/assets/ea362c19-8004-47c9-b801-7c0387b54a96)

This process is repeated for all elements of matrix (C).

# **Identity and Diagonal matrix**

![image](https://github.com/user-attachments/assets/61ab59b7-ee78-4459-888a-7d46bbafd20b)


