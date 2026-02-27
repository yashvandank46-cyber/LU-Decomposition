# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program.
2. Read the input matrix A and (if required) matrix B.
3. Perform LU decomposition on matrix A to obtain L and U, and use them to solve AX = B.
4. Display the matrices L, U and the solution matrix X, then stop.

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: YASHVANDAN K
RegisterNumber: 212225100060'''

import numpy as np
from scipy.linalg import lu
a=np.array(eval(input()))
b,c,d=lu(a)
print(c)
print(d)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: YASHVANDAN K
RegisterNumber: 212225100060
'''
# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(a)
x=lu_solve((lu,piv),b)
print(x)

```

## Output:
![alt text](<Screenshot 2026-02-27 220513.png>)
![alt text](<Screenshot 2026-02-27 221310.png>)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

