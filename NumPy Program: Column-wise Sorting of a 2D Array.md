# NumPy Program: Column-wise Sorting of a 2D Array

## 🎯 Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

## 🧠 Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

## 🧾 Program

~~~
import numpy as np

r = int(input("Enter number of rows: "))
c = int(input("Enter number of columns: "))

data = []

print("Enter elements:")
for i in range(r):
    row = list(map(int, input().split()))
    data.append(row)

arr = np.array(data)

sorted_arr = np.sort(arr, axis=0)

print("Original array:")
print(arr)

print("Column-wise sorted array:")
print(sorted_arr)
~~~

## Output

<img width="652" height="553" alt="image" src="https://github.com/user-attachments/assets/ae326f1c-886a-4f7e-b1d1-1b05d84bc7fd" />


## Result

The NumPy program to sort the elements of a 2D array column-wise in ascending order was executed successfully and the output was verified.
