# Norm of a matrix
## Aim
To write a program to find the 1-norm, 2-norm and infinity norm of the matrix and display the result in two decimal places.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
 # 1-norm
 ```
1.Input the Array: Read the input for the array (vector or matrix) from the user.
2.Convert to NumPy Array: Parse the input into a NumPy array for numerical operations.
3.Compute the 1-Norm: Use np.linalg.norm with the ord=1 parameter to calculate the 1-norm.
4.Format the Result: Format the calculated 1-norm to two decimal places for better readability.
5.Output the Result: Print the formatted 1-norm value.
6.End Program: Ensure the program ends cleanly after displaying the result.

```
# 2-norm
```
1.Input the Array: Read the input for the array (vector or matrix) from the user.
2.Convert to NumPy Array: Parse the input into a NumPy array for numerical computations.
3.Compute the 2-Norm: Use np.linalg.norm with the ord=2 parameter (default) to calculate the 2-norm.
4.Format the Result: Format the calculated 2-norm to two decimal places for better readability.
5.Output the Result: Print the formatted 2-norm value.
6.End Program: Ensure the program concludes after displaying the result.

```
# infinity norm
```
1.Input the Matrix: Read the input matrix from the user.
2.Convert to NumPy Array: Parse the input into a NumPy array for numerical operations.
3.Compute Row Sums: For each row in the matrix, compute the sum of the absolute values of its elements.
4.Find Maximum Row Sum: Identify the largest row sum among all rows.
5.Format the Result: Format the calculated infinity norm (maximum row sum) to two decimal places.
6.Output the Result: Print the formatted infinity norm value.

```



## Program:
```Python
# Register No: 24901278
# Developed By: shakthivel v
# 1-Norm of a Matrix
import numpy as np
arr = np.array(eval(input()))
result =np.linalg.norm (arr,1)
print ("{:.2f}".format(result))



# Developed By: Shakthivel v
# Register No:24901278
# 2-Norm of a Matrix
import numpy as np
arr=np.array(eval(input()))
result=np.linalg.norm(arr,2)
print("{:.2f}".format(result))


# Developed By : Shakthivel v
# Register No: 24901278
# Infinity Norm of a Matrix
import numpy as np
def infinity_norm(matrix):
    max_row_sum = max(sum(abs(element) for element in row)for row in matrix)
    return max_row_sum
matrix=np.array(eval(input()))
result=infinity_norm(matrix)
print(f"{result:.2f}")

```
## Output:
### 1-Norm of a Matrix

![alt text](<Screenshot 2024-12-06 231252.png>)


### 2-Norm of a Matrix
![alt text](<Screenshot 2024-12-06 231427.png>)

### Infinity Norm of a Matrix
![alt text](<Screenshot 2024-12-06 231452.png>)

## Result
Thus the program for 1-norm, 2-norm and Infinity norm of a matrix are written and verified.
