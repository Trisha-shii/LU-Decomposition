# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program
2. Import the necessary libraries(numpy,scipy.linalg)
3. Define the matrix using numpy
4. Use lu(),lu_solve(),lu_factor() to get the solutions
5. End the program

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: TRISHA PRIYADARSHNI PARIDA
RegisterNumber: 212224230293
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu

A  = np.array(eval(input()))
P,L,U = lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: TRISHA PRIYADARSHNI PARIDA 
RegisterNumber: 212224230293
'''

import os
os.environ["OPENBLAS_NUM_THREADS"]="1"

# To print X matrix (solution to the equations)
import numpy as np

from scipy.linalg import lu_factor, lu_solve

A = np.array(eval(input()))
B = np.array(eval(input()))

l,p = lu_factor(A)

X = lu_solve((l,p),B)

print(X)


```

## Output:
![lu decomposition]()

<img width="1919" height="996" alt="image" src="https://github.com/user-attachments/assets/3378b0ec-96f9-49cb-96c2-80b3a4d1e9a5" />
<img width="1918" height="765" alt="image" src="https://github.com/user-attachments/assets/75e5393a-c6ec-4383-8028-88cf874a7972" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

