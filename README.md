# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. import numpy 
2. import sys
3. get the input from the users
4. use nested for loop
5. print the solved matrix using gaussian elemination without partial pivoting

## Program:
```python
'''
Program to find the solution of a matrix using Gaussian Elimination.
Developed by: yuvabharathib
RegisterNumber: 22002787
import numpy as np
import sys
n=int(input())
a=np.zeros((n,n+1)) 
x=np.zeros
for i in range(n):
    for j in range (n+1):
        a[i][j]=float(input())
    #print(a)
for i in range(n):
    if a[i][j]==0.0:
        sys. exit('Divide by zero found!')
        
    for j in range(i+1,n):
        scalar=a[j][i]/a[i][i]
        
        for k in range(n+1):
            a[j][k]=a[j][k]-scalar*a[i][k]
x[n-1]=a[n-1][n]/a[n-1][n-1]
for i in range(n-2, -1,-1):
    x[i]=a[i][n]
    for j in range(i+1,n):
        x[i]=x[i]-a[i][j]*x[j]
    x[i]=x[i]/a[i][i]
for i in range(n):
    print('X%d = %0.2f'%(i,x[i]),end=' ')
```
## Output:
![gaussian elemination](https://user-images.githubusercontent.com/113497406/192081482-e6067f86-90ef-494d-a77d-6bf21c70b1cf.png)

## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.
