# Multi-Dimensional Arrays
A multidimensional array is an array that contains more than one dimension, allowing you to store data in a grid-like structure or higher dimensions. Essentially, it's an array of arrays. The most common type of multidimensional array is the two-dimensional array, but you can have arrays with three, four, or more dimensions.

Key Characteristics:
- **Multiple Dimensions**: Arrays can have two, three, or more dimensions.
- **Homogeneous Elements**: All elements in the array are of the same type.
- **Contiguous Memory**: The elements are stored in contiguous memory locations.
- **Indexing**: Elements are accessed using multiple indices, one for each dimension.

## Creating, Traversing, and Modifying a Two-Dimensional Array in C++
```cpp
#include <iostream>
using namespace std;

int main() {
    // Declaring and initializing a 2D array with 3 rows and 4 columns
    int matrix[3][4] = {
        {1, 2, 3, 4},
        {5, 6, 7, 8},
        {9, 10, 11, 12}
    };

    // Accessing and printing elements of the 2D array
    cout << "Element at [1][2]: " << matrix[1][2] << endl; // Output: 7

    // Looping through the 2D array to print all elements
    cout << "All elements in the 2D array:" << endl;
    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 4; j++) {
            cout << matrix[i][j] << " ";
        }
        cout << endl; // Moves to the next row
    }

    return 0;
}
```
1. Array Declaration and Initialization:
    - `int matrix[3][4] = { ... };`: Here, a two-dimensional array named `matrix` is declared and initialized. It has 3 rows and 4 columns. Each element of the array is specified in a nested list:
        * The first row contains `{1, 2, 3, 4}`
        * The second row contains `{5, 6, 7, 8}`
        * The third row contains `{9, 10, 11, 12}`
2. Accessing and Printing Elements:
    - `matrix[1][2]`: This accesses the element at the second row (index 1) and third column (index 2) of the `matrix`. The value at this position is `7`.
    - `cout << "Element at [1][2]: " << matrix[1][2] << endl;`: This prints the value of the accessed element. The output will be `Element at [1][2]: 7`.
3. Looping through the 2D Array:
    - `cout << "All elements in the 2D array:" << endl;`: This prints a header message before displaying all the elements of the array.
    - `for (int i = 0; i < 3; i++) { ... }`: This outer loop iterates through each row of the `matrix` (from row 0 to row 2).
    - `for (int j = 0; j < 4; j++) { ... }`: This inner loop iterates through each column of the current row (from column 0 to column 3).
    - `cout << matrix[i][j] << " ";`: This prints the element at the current row `i` and column `j`, followed by a space.
    - `cout << endl;`: After printing all elements in a row, this moves the cursor to the next line, effectively creating a new line for the next row.
