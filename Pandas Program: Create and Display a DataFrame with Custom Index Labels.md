# Pandas Program: Create and Display a DataFrame with Custom Index Labels

## 🎯 Aim

To create and display a **DataFrame** using the **Pandas** library in Python from a given dictionary, and apply specific index labels to the rows.

---

## 🧠 Algorithm

1. **Import Libraries**: Import the required libraries – `pandas` and `numpy`.
2. **Create Dictionary**: Define a dictionary `exam_data` with keys: `'name'`, `'score'`, `'attempts'`, and `'qualify'`.
3. **Index Labels**: Create a list of custom index labels called `labels`.
4. **Create DataFrame**: Use `pd.DataFrame()` to create the DataFrame by passing the dictionary and index labels.
5. **Display Output**: Display the DataFrame using `print()` or by simply calling the DataFrame variable.

---

## 💻 Program
    import pandas as pd
    import numpy as np
    
    # Step 2: Create dictionary
    exam_data = {
        'name': ['Anastasia', 'Dima', 'Katherine', 'James', 'Emily'],
        'score': [12.5, 9, 16.5, np.nan, 9],
        'attempts': [1, 3, 2, 3, 2],
        'qualify': ['yes', 'no', 'yes', 'no', 'no']
    }
    
    # Step 3: Define custom index labels
    labels = ['a', 'b', 'c', 'd', 'e']
    
    # Step 4: Create DataFrame
    df = pd.DataFrame(exam_data, index=labels)
    
    # Step 5: Display DataFrame
    print("Custom Indexed DataFrame:\n")
    print(df)


## Output
    Custom Indexed DataFrame:
    
            name  score  attempts qualify
    a  Anastasia   12.5         1     yes
    b       Dima    9.0         3      no
    c  Katherine   16.5         2     yes
    d      James    NaN         3      no
    e      Emily    9.0         2      no


## Result
The program successfully creates and displays a Pandas DataFrame with the specified custom row index labels.
