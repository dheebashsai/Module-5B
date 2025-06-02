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
    import numpy as np
    
    # Step 2: Define a 2D NumPy array (can be replaced with user input if needed)
    arr = np.array([[12, 5, 7],
                    [3, 8, 1],
                    [6, 4, 9]])
    
    # Step 3 & 4: Sort column-wise
    sorted_arr = np.sort(arr, axis=0)
    
    # Step 5: Display output
    print("Original Array:\n", arr)
    print("\nColumn-wise Sorted Array:\n", sorted_arr)

## Output
    Original Array:
     [[12  5  7]
     [ 3  8  1]
     [ 6  4  9]]
    
    Column-wise Sorted Array:
     [[ 3  4  1]
     [ 6  5  7]
     [12  8  9]]

## Result
The program successfully performs column-wise sorting of the 2D array using NumPy.
