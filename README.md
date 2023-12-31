# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
(i)
1.Import lu from scipy.linalg package
2.Import numpy module
3.Create the matrix
4.Use lu to find the L and U matrix
5.Print the L and U matrix

(ii)
1.Import lu_factor and lu_solve from scipy.linalg package
2.Import numpy module
3.Create the matrix
4.Take a constant as input
5.Use lu_factor to find the factor
6.Use lu_solve to find the solution
7.Print the solution

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: Shehan Shajahan
RegisterNumber: 23008724
*/
#To print L and U matrix
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
Developed by: Shehan Shajahan 
RegisterNumber: 23008724 
*/
# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(A)
x=lu_solve((lu,piv),b)
print(x)
```
## Output:
![Screenshot 2023-12-31 193655](https://github.com/shehanshajahan/LU-Decomposition/assets/139317389/fe9b248d-4d27-4749-963c-562ea6de6047)
![Screenshot 2023-12-31 193718](https://github.com/shehanshajahan/LU-Decomposition/assets/139317389/53928eaa-350e-4db4-a360-dab2da0e164b)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

