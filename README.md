# INVERSE-OF-A-MATRIX
## Aim:
To write a python program to find the inverse of a matrix
## Equipment’s required:
1. 	Hardware – PCs
2. 	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1 : 
### Step 2: 
### Step 3: 
### Step 4: 

## Program:
    import numpy as np

def find_inverse(matrix):
    # Convert the matrix into a NumPy array
    matrix = np.array(matrix)
    
    # Check if the matrix is square
    if matrix.shape[0] != matrix.shape[1]:
        raise ValueError("Matrix is not square and cannot have an inverse.")
    
    # Compute the determinant
    determinant = np.linalg.det(matrix)
    if determinant == 0:
        raise ValueError("Matrix is singular and does not have an inverse.")
    
    # Compute the inverse
    inverse_matrix = np.linalg.inv(matrix)
    return inverse_matrix

# Given matrix
matrix = [
    [2, 1, 1],
    [1, 1, 1],
    [1, -1, 2]
]

try:
    # Find and print the inverse
    inverse = find_inverse(matrix)
    print(inverse)
except ValueError as e:
    print(e)

## Output:![output image](<Untitled design.png>)
## Result:
Thus the inverse of given matrix is successfully solved using python program

