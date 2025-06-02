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
    import numpy as np
    
    # Step 2: Define the original 2D array
    original_array = np.array([[1, 2, 3],
                               [4, 5, 6],
                               [7, 8, 9]])
    
    # New column to insert
    new_column = np.array([10, 11, 12])
    
    # Step 3: Delete the second column (index 1)
    array_without_second_col = np.delete(original_array, 1, axis=1)
    
    # Step 4: Insert the new column at index 1
    updated_array = np.insert(array_without_second_col, 1, new_column, axis=1)
    
    # Step 5: Display the result
    print("Original Array:\n", original_array)
    print("\nNew Column:", new_column)
    print("\nUpdated Array:\n", updated_array)


## Output
    Original Array:
     [[1 2 3]
     [4 5 6]
     [7 8 9]]
    
    New Column: [10 11 12]
    
    Updated Array:
     [[ 1 10  3]
     [ 4 11  6]
     [ 7 12  9]]


## Result
The program successfully replaces the second column of the 2D array with the provided new column.
