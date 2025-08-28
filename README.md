# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm

1.Start with a square matrix A of order n × n.

2.Decompose A into L (lower triangular with 1’s on diagonal) and U (upper triangular).

3.Compute entries of U row-wise and L column-wise using elimination.

4.Finally, verify that A = L × U.

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: Janani Gowrisankar
RegisterNumber: 212224100022
*/

import numpy as np
from scipy.linalg import lu
a=np.array(eval(input()))
p,l,u=lu(a)
print(l)
print(u)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: Janani Gowrisankar
RegisterNumber: 212224100022
*/

import numpy as np
from scipy.linalg import lu_factor, lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
l,p=lu_factor(a)
x=lu_solve((l,p),b)
print(x)

```
## Output:
(i) To find the L and U matrix


<img width="1184" height="965" alt="image" src="https://github.com/user-attachments/assets/8e5f680a-bb4a-424d-8810-dbef3b66298f" />

(ii) To find the LU Decomposition of a matrix


<img width="1185" height="750" alt="image" src="https://github.com/user-attachments/assets/7407bb6f-3c46-4431-93aa-ac5497986788" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

