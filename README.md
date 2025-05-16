# Norm of a matrix
## Aim
To write a program to find the 1-norm, 2-norm and infinity norm of the matrix and display the result in two decimal places.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
	1. Get the input matrix using np.array()   
    2. Find the 2-norm of the matrix using np.linalg.norm()
	3. Print the norm of the matrix in two decimal places.
## Program:
```
# Register No: 212224240170
# Developed By: THARRUN D
# 1-Norm of a Matrix


def one_norm(matrix):
   
    columns = list(zip(*matrix))
    max_col_sum = max(sum(abs(x) for x in col) for col in columns)
    print(f"{max_col_sum:.2f}")


matrix =eval(input())
one_norm(matrix)

# 2-Norm of a Matrix

'''
Program to find 2-norm of a matrix.
Developed by: THARRUN D
RegisterNumber: 212224240170
'''
import numpy as n
a=n.array(eval(input()))
b=n.linalg.norm(a,2)
no="{:.2f}".format(b)
print(no)

# Infinity Norm of a Matrix

def infinity_norm(matrix):
    max_row_sum = max(sum(abs(x) for x in row) for row in matrix)
    print(f"{max_row_sum:.2f}")


matrix = eval(input())
infinity_norm(matrix)
```
## Output:
### 1-Norm of a Matrix

![Screenshot 2025-05-17 000815](https://github.com/user-attachments/assets/197b9322-1bb0-454d-9701-70ed61d1d4ff)


### 2-Norm of a Matrix

![Screenshot 2025-05-17 000830](https://github.com/user-attachments/assets/fff59a22-4518-420c-b91a-960fabb0a8f1)



### Infinity Norm of a Matrix


![Screenshot 2025-05-17 000848](https://github.com/user-attachments/assets/7eecc0c0-3bd2-4a42-b107-54480e88285b)




## Result
Thus the program for 1-norm, 2-norm and Infinity norm of a matrix are written and verified.
