# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### Step 1: 
Import the numpy module to use the built-in functions for calculation
### Step 2: 
Prepare the lists from each linear equations and assign in np.array()
### Step 3: 
Using the np.linalg.solve(), we can find the solutions.
### Step 4: 
End the program

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: SANJAI S J
RegisterNumber: 212225040365
'''
import os  
os.environ["OPENBLAS_NUM_THREADS"]="1" 
import numpy as np
from scipy.linalg import lu 
A=np.array(eval(input()))
P,L,U=lu(A) 
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: SANJAI S J
RegisterNumber: 212225040365
'''

# To print X matrix (solution to the equations)
import os 
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np 
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,pivot= lu_factor(A)
x=lu_solve((lu,pivot),B)
print(x)
```

## Output:

<img width="1187" height="444" alt="image" src="https://github.com/user-attachments/assets/12619744-ef08-48f5-922a-058b4fc35855" />

<img width="1099" height="183" alt="image" src="https://github.com/user-attachments/assets/5370a87f-1939-4230-a9f4-6fb80c700906" />

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

