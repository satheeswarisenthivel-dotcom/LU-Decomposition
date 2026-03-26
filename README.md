# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.FINDING THE 'L' AND 'U' MATRIX : STEP1 : Import the numpy module to use the built-in functions for calculation.

STEP2 : Prepare the lists from each linear equations and assign in np.array().

STEP3 : Using the P,L,U =lu(), we get two results (first is L and second is U) of the given matrix.

STEP4 : end the program

2.FINDING DECOMPOSITION OF THE MATRIX:

STEP1 : Import the numpy module to use the built-in functions for calculation.

STEP2 : Prepare the lists from each linear equations and assign in np.array().

STEP3 : Using the pivot=lu_factor(A) andx=lu_solve((lu,pivot),B) , we can find results the LU Decomposition of a matrix

STEP4 : end the program 

## Program:
(i) To find the L and U matrix
```
import numpy as np
from scipy.linalg import lu
matrix=np.array(eval(input()))
P,L,U=lu(matrix)
print(L)
print(U)
/*
Program to find the L and U matrix.
Developed by: SATHEESWARI .S 
RegisterNumber: 212225240141
*/
```
(ii) To find the LU Decomposition of a matrix
```
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A = np.array(eval(input()))
B = np.array(eval(input()))
lu,piv = lu_factor(A)
X = lu_solve((lu,piv),B)
print(X)
/*
Program to find the LU Decomposition of a matrix.
Developed by: SATHEESWARI.S
RegisterNumber: 212225240141
*/
```


## Output:

<img width="998" height="394" alt="Screenshot 2026-03-26 112353" src="https://github.com/user-attachments/assets/3b6255d7-bb53-4c9a-8318-d9b06c3aa8d7" />

<img width="1013" height="450" alt="Screenshot 2026-03-16 220508" src="https://github.com/user-attachments/assets/eebbc0a3-b891-4ce4-9728-e6af5c1272aa" />

<img width="783" height="265" alt="Screenshot 2026-03-16 220358" src="https://github.com/user-attachments/assets/d157461d-a09e-4df8-9fa5-3b7bd540a639" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

