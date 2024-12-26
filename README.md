# Norm of a matrix
## Aim
To write a program to find the 1-norm, 2-norm and infinity norm of the matrix and display the result in two decimal places.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
 # 1-norm
 ```
1. Import Libraries: Import numpy as np for numerical computations.
2.Take Input: Accept a user-provided array or matrix as input and evaluate it using eval().
3.Convert to NumPy Array: Convert the evaluated input to a NumPy array using np.array().
4.Compute 1-Norm: Use np.linalg.norm(arr, 1) to calculate the 1-norm.
5.Format the Result: Format the computed norm to two decimal places using "{:.2f}".format().
6.Output Result: Print the formatted result to the console.
7.Ensure Valid Input: Input should be a valid array or matrix (automatically handled).
8.Handle Errors: Errors in input or computation will result in an exception being raised.
```
# 2-norm
```
1.Import Library: Import the numpy library for numerical computations.
2.Input Array: Accept user input, evaluate it, and convert it into a NumPy array using np.array().
3.Calculate 1-Norm: Use np.linalg.norm(arr, 1) to compute the 1-norm of the array or matrix.
4.Format Result: Format the computed norm to two decimal places using "{:.2f}".format().
5.Output Result: Print the formatted result to the console.
6.Handle Errors: Ensure valid input and let the program raise exceptions for invalid cases.
```
# infinity norm
```
1.Import Library: Import numpy as np for working with numerical arrays.
2.Define Function: Define the function infinity_norm(matrix) to compute the infinity norm of a matrix.
3.Calculate Absolute Values: Within the function, compute the absolute value of each element in the matrix.
4.Compute Row Sums: Calculate the sum of the absolute values of elements in each row of the matrix.
5.Find Maximum Row Sum: Determine the maximum row sum, which represents the infinity norm.
6.Take Input Matrix: Accept user input, evaluate it, and convert it to a NumPy array using np.array().
7.Call Function: Pass the input matrix to the infinity_norm function and store the result.
8.Format and Print Result: Format the result to two decimal places and print it.
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
