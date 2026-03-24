# NumPy Program: Replace the Second Column in a 2D Array

## 🎯 Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

## 🧠 Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

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

arr_deleted = np.delete(arr, 1, axis=1)

new_col = list(map(int, input("Enter new column values: ").split()))

updated_arr = np.insert(arr_deleted, 1, new_col, axis=1)

print("Updated array:")
print(updated_arr)
~~~

## Output

<img width="680" height="542" alt="image" src="https://github.com/user-attachments/assets/22daa931-24e5-439a-bac3-4c2ceff3da5c" />

## Result:

The NumPy program to delete the second column and insert a new column in a 2D array was executed successfully and the output was verified.

## Result
