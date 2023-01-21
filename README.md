# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import numpy library using import statement.
2. From scripy package import lu_factor() and lu_solve().
3. Get two inputs from user andpasss it as matrix array.
4. Find lu and pivot value of first matrix using lu_factor().
5. Find solution of thematrix by using lu_solve() by passing lu.pivot values as first argument and second matrix as second argument.

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: Premalatha.S
RegisterNumber: 22009393
*/
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: Premalatha.S
RegisterNumber: 22009393
*/
# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv = lu_factor(A)
x=lu_solve((lu,piv),b)
print(x)
```

## Output:
![image](https://user-images.githubusercontent.com/120620842/213876710-08351ec5-f819-4793-a0a1-c98ccfb0475e.png)

![image](https://user-images.githubusercontent.com/120620842/213876753-fa9dc377-6c46-41e9-b7f9-3aec2ae54b56.png)



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

