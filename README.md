# EX-5 LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## ()Algorithm
### Step 1:  
Import required libraries `numpy` and `scipy.linalg`.  

### Step 2:  
Input the matrix/matrices using `eval(input())`.  

### Step 3:  
Perform LU decomposition using `lu()` or solve equations using `lu_factor()` and `lu_solve()`.  

### Step 4:  
Print the results `L` and `U` matrices or solution `X` matrix.

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: Vignesh V
RegisterNumber: 21224040357
'''
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: Vigensh V
RegisterNumber: 212224040357
'''

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,pivot=lu_factor(A)
x=lu_solve((lu,pivot),B)
print(x) 
```

## Output:
(i) To find the L and U matrix
<img width="1313" height="970" alt="image" src="https://github.com/user-attachments/assets/290fffe5-e05b-429b-9b0f-8995ae8ab963" />

(ii) To find the LU Decomposition of a matrix
<img width="1328" height="794" alt="image" src="https://github.com/user-attachments/assets/4367632d-69d0-467d-96fd-86928c6bc254" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

