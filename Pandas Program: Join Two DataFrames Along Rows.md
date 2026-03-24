# 🧪 Pandas Program: Join Two DataFrames Along Rows

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

---

## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

---

## 💻 Program

~~~
import pandas as pd

student_data1 = {
    'id': [1, 2, 3],
    'name': ['John', 'Alex', 'Anna'],
    'marks': [85, 90, 78]
}

student_data2 = {
    'id': [4, 5, 6],
    'name': ['Mike', 'Sara', 'David'],
    'marks': [88, 92, 80]
}

df1 = pd.DataFrame(student_data1)
df2 = pd.DataFrame(student_data2)

new_df = pd.concat([df1, df2], axis=0)

print(new_df)
~~~

## Output

<img width="629" height="454" alt="image" src="https://github.com/user-attachments/assets/c1677e1e-d23f-422e-aef0-4787eda0437c" />


## Result

The Pandas program to join two DataFrames along rows was executed successfully and the output was verified.
