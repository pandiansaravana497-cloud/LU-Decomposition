# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
## (i) To find the L and U matrix

### Step 1:
Start.
### Step 2:
Input the matrix 𝐴,A from the user.
### Step 3:
Store the matrix as a NumPy array.
### Step 4:
Call the LU decomposition function from scipy.linalg.lu(A) which decomposes 
the matrix into three matrices:
P: Permutation matrix
L: Lower triangular matrix
U: Upper triangular matrix
### Step 5:
Extract P, L, and U from the function output.
### Step 6:
Display the L (lower triangular matrix).
Display the U (upper triangular matrix).
### Step 7:
End.
## (ii) To find the LU Decomposition of a matrix

### Step 1:
Start
### Step 2:
Input the coefficient matrix A.
### Step 3:
Input the constant matrix (right-hand side vector) B.
### Step 4:
Perform LU factorization of matrix A using lu_factor(A), which returns:
A combined matrix containing the factors of L and U.
A pivoting array P representing row interchanges.
### Step 5:
Solve the system of equations AX=B using the LU factors and the pivoting array with lu_solve((L, P), B).
### Step 6:
Store the result in variable X.
### Step 7:
Print the solution vector X. 
### Step 8:
End


## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: PON SARAVANA PANDIAN B
RegisterNumber: 212225230207
import numpy as np
from scipy.linalg import lu

a = np.array(eval(input()))
p,l,u = lu(a)
print(l)
print(u)
*/
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: PON SARAVANA PANDIAN B
RegisterNumber: 212225230207
import numpy as np
from scipy.linalg import lu_factor,lu_solve

A = np.array(eval(input()))
B = np.array(eval(input()))

L,P=lu_factor(A)
X = lu_solve((L,P),B)

print(X)

*/
```

## Output:
<img width="1144" height="794" alt="image" src="https://github.com/user-attachments/assets/356f0267-0b21-44b0-9579-e6c4e1d2a072" />

<img width="801" height="639" alt="image" src="https://github.com/user-attachments/assets/aa3cb4fe-23c6-44cd-960d-5f5014acebea" />





## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

