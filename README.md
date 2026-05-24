# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the required library and define the matrix.
2. Use the LU decomposition function to decompose the matrix into Lower triangular matrix L and Upper triangular matrix U.
3. Store the matrices L and U in separate variables.
4. Display the matrices L and U.

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: S.KEERTHANA
RegisterNumber: 212225040186
*/

import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A = eval(input())
a = np.array(A)
P, L, U = lu(A)
print(L)
print(U)
            
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: S.KEERTHANA
RegisterNumber: 212225040186
*/

import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A = np.array(eval(input()))
B = np.array(eval(input()))
lu, piv = lu_factor(A)
X = lu_solve((lu, piv), B)
print(X)
```

## Output:
<img width="1229" height="822" alt="image" src="https://github.com/user-attachments/assets/7d10fad3-01de-4f29-b285-7d5e9299c205" />

<img width="1259" height="574" alt="image" src="https://github.com/user-attachments/assets/bfb775ef-6690-41d8-b6cd-1b6206888a06" />

<img width="1197" height="797" alt="image" src="https://github.com/user-attachments/assets/b40b58b9-6b61-437b-8a9f-e0fc3ef27ebf" />

<img width="1082" height="248" alt="image" src="https://github.com/user-attachments/assets/7d042775-a753-4ade-b1c2-c9844f94cd46" />

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

