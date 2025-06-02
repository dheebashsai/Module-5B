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
    import pandas as pd
    
    # Step 2: First DataFrame
    student_data1 = {
        'student_id': ['S1', 'S2', 'S3', 'S4'],
        'name': ['Alice', 'Bob', 'Charlie', 'David'],
        'marks': [85, 90, 95, 80]
    }
    df1 = pd.DataFrame(student_data1)
    
    # Step 3: Second DataFrame
    student_data2 = {
        'student_id': ['S5', 'S6'],
        'name': ['Eva', 'Frank'],
        'marks': [88, 92]
    }
    df2 = pd.DataFrame(student_data2)
    
    # Step 4: Concatenate row-wise
    combined_df = pd.concat([df1, df2], axis=0, ignore_index=True)
    
    # Step 5: Display the result
    print("Combined DataFrame:\n")
    print(combined_df)

## Output
    Combined DataFrame:
    
      student_id     name  marks
    0         S1    Alice     85
    1         S2      Bob     90
    2         S3  Charlie     95
    3         S4    David     80
    4         S5      Eva     88
    5         S6     Frank     92


## Result
The program successfully concatenates two DataFrames along rows, producing a unified DataFrame with continuous indexing.


