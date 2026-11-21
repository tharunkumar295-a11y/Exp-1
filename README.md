# Experiment 1: Exploring NumPy and Pandas

## Aim

To understand the use of NumPy and Pandas for performing basic data
manipulation and analysis in Python.

## Algorithm

1.  Import the NumPy library for matrix and numerical operations.
2.  Define a two-dimensional square matrix `A` and a vector `b`.
3.  Compute the transpose of matrix `A` to interchange rows and columns.
4.  Calculate the inverse of matrix `A` using `np.linalg.inv(A)` (ensure
    `A` is non-singular).
5.  Solve the linear equation `A × x = b` using `np.linalg.solve(A, b)`.
6.  Perform eigen decomposition to find eigenvalues and eigenvectors
    using `np.linalg.eig(A)`.
7.  Display the results for the matrix, transpose, inverse, solution
    vector, and eigenvalues.
8.  End the program.

## Formulas / Theory

-   **Transpose:** `Aᵀ` --- interchange rows and columns.
-   **Inverse:** `A⁻¹ = adj(A) / |A|`, provided `det(A) ≠ 0`.
-   **Linear system:** `A × x = b  ⇒  x = A⁻¹b`.
-   **Eigen decomposition:** `A v = λ v`, where `λ` is an eigenvalue and
    `v` is an eigenvector.

## Coding
# Experiment 1: Exploring NumPy and Pandas

# Import libraries
import numpy as np
import pandas as pd

# Define a square matrix A and vector b
A = np.array([[4, 2],
              [1, 3]])

b = np.array([10, 8])

# Display Matrix A
print("Matrix A:")
print(A)

# Compute transpose
A_transpose = A.T
print("\nTranspose of A:")
print(A_transpose)

# Compute inverse
A_inverse = np.linalg.inv(A)
print("\nInverse of A:")
print(A_inverse)

# Solve linear system Ax = b
x = np.linalg.solve(A, b)
print("\nSolution of Ax = b:")
print(x)

# Eigen decomposition
eigenvalues, eigenvectors = np.linalg.eig(A)

print("\nEigenvalues:")
print(eigenvalues)

print("\nEigenvectors:")
print(eigenvectors)

# Demonstration of Pandas
df = pd.DataFrame(A, columns=['Column1', 'Column2'])

print("\nPandas DataFrame:")
print(df)

print("\nDescriptive Statistics:")
print(df.describe())

## Output
<img width="372" height="570" alt="image" src="https://github.com/user-attachments/assets/784873ad-275b-4361-b148-d4cdf66521c6" />
<img width="348" height="232" alt="image" src="https://github.com/user-attachments/assets/5709ecfa-68a4-4bb6-8062-d0b899af6c46" />


## Result
NumPy was successfully used to perform matrix operations such as transpose, inverse computation, solving a system of linear equations, and eigen decomposition. Pandas was used to create a DataFrame and perform basic data analysis using descriptive statistics. Thus, the use of NumPy and Pandas for data manipulation and numerical computation was successfully explored.
