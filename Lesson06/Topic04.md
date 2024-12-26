# Array Traversal
Array traversal is the process of accessing and processing each element of an array, typically in a sequential manner. This operation is fundamental in programming because it allows you to examine, modify, or utilize each element within the array.

### Tips for Array Traversal in C++
1. Efficient Looping:
- Tip: Optimize your loop conditions to minimize repeated calculations.
- Example: Store the length of the array in a variable instead of calculating it in every loop iteration.
```cpp
int length = sizeof(arr) / sizeof(arr[0]);
for (int i = 0; i < length; i++) {
    // Process arr[i]
}
```
2. Boundary Checking:
- Tip: Always check your loop boundaries to avoid accessing out-of-bounds elements, which can lead to undefined behavior.
- Example: Use conditions to ensure the loop index remains within the valid range of the array.
```cpp
int i = 0;
while (i < length) {
    if (i >= 0 && i < length) {
        // Process arr[i]
    }
    i++;
}
```
3. Nested Loop Traversal:
- Tip: For multidimensional arrays, use nested loops carefully to ensure all elements are accessed correctly.
- Example: Nested loops for 2D or 3D arrays should accurately reflect the structure of the array.
```cpp
for (int i = 0; i < rows; i++) {
    for (int j = 0; j < cols; j++) {
        // Process matrix[i][j]
    }
}
```
4. Conditional Traversal:
- Tip: Use conditions within your loops to filter or modify specific elements based on criteria.
- Example: Apply a condition to only process even numbers in the array.
```cpp
for (int i = 0; i < length; i++) {
    if (arr[i] % 2 == 0) {
        // Process even elements
    }
}
```
5. Use do-while for Guaranteed Execution:
- Tip: Use a do-while loop when you need the loop to run at least once, regardless of the condition.
- Example: Useful for scenarios where you must process at least the first element before further conditions.
```cpp
int i = 0;
do {
    // Process arr[i]
    i++;
} while
```
---

## Traversing a One-Dimensional Array Using a For Loop and sizeof in C++
```cpp
#include <iostream>
using namespace std;

int main() {
    // Declaring and initializing a 1D array
    int arr[] = {10, 20, 30, 40, 50};

    // Calculating the number of elements in the array using sizeof
    int size = sizeof(arr) / sizeof(arr[0]);

    // Traversing the 1D array using a for loop
    cout << "Elements of the array are: ";
    for (int i = 0; i < size; i++) {
        cout << arr[i] << " "; // Access and print each element
    }
    cout << endl; // Move to the next line after printing all elements

    return 0;
}
```

1. Array Declaration and Initialization:
   - Declares and initializes a one-dimensional array named `arr` with 5 integer elements: `{10, 20, 30, 40, 50}`.
```cpp
int arr[] = {10, 20, 30, 40, 50};
```

2. Calculating Array Size Using `sizeof`:
    - `sizeof(arr)` gives the total size of the array in bytes.
    - `sizeof(arr[0])` gives the size of the first element in bytes.
    - `sizeof(arr) / sizeof(arr[0])` calculates the number of elements in the array.
```cpp
int size = sizeof(arr) / sizeof(arr[0]);
```

3. Traversing the Array Using a For Loop:
    - The `for` loop initializes `i` to 0.
    - The loop condition `i < size` ensures the loop runs until i reaches the size of the array.
    - `arr[i]` accesses the element at index `i` and `cout << arr[i] << " ";` prints each element followed by a space.
```cpp
for (int i = 0; i < size; i++) {
    cout << arr[i] << " "; // Access and print each element
}
```

This example demonstrates C++ program that uses a `for` loop to traverse a one-dimensional array and the `sizeof` operator to determine the array's size.

---

## Traversing a One-Dimensional Array Using a While Loop and sizeof in C++
```cpp
#include <iostream>
using namespace std;

int main() {
    // Declaring and initializing a 1D array
    int arr[] = {10, 20, 30, 40, 50};

    // Calculating the number of elements in the array using sizeof
    int length = sizeof(arr) / sizeof(arr[0]);

    // Traversing the 1D array using a while loop
    int i = 0; // Initialization
    cout << "Elements of the array are: ";
    while (i < length) { // Condition
        if (i >= 0 && i < length) { // Boundary check
            cout << arr[i] << " "; // Access and print each element
        }
        i++; // Increment
    }
    cout << endl; // Move to the next line after printing all elements

    return 0;
}
```
1. Array Declaration and Initialization:
    - Declares and initializes a one-dimensional array named arr with 5 integer elements: `{10, 20, 30, 40, 50}`.
```cpp
int arr[] = {10, 20, 30, 40, 50};
```
2. Calculating Array Size Using sizeof:
    - `sizeof(arr)` gives the total size of the array in bytes.
    - `sizeof(arr[0])` gives the size of the first element in bytes.
    - `sizeof(arr) / sizeof(arr[0])` calculates the number of elements in the array.
```cpp
int length = sizeof(arr) / sizeof(arr[0]);
```

3. Traversing the Array Using a While Loop:
    - Initializes `i` to 0.
    - The `while` loop runs as long as `i` is less than `length` (the number of elements in the array).
    - The `if` condition ensures that `i` is within valid bounds.
    - `cout << arr[i] << " ";` accesses and prints each element.
    - `i++` increments the index to move to the next element.
```cpp
int i = 0; // Initialization
cout << "Elements of the array are: ";
while (i < length) { // Condition
    if (i >= 0 && i < length) { // Boundary check
        cout << arr[i] << " "; // Access and print each element
    }
    i++; // Increment
}
cout << endl; // Move to the next line after printing all elements
```
This example demonstrates how to use a `while` loop to traverse a one-dimensional array in C++, including boundary checking to ensure safe access to array elements.

## Calculating the Sum of a Two-Dimensional Array with User Input Using Nested For Loops and sizeof in C++
```cpp
#include <iostream>
using namespace std;

int main() {
    int rows, cols;

    // Ask user for the dimensions of the array
    cout << "Enter the number of rows: ";
    cin >> rows;
    cout << "Enter the number of columns: ";
    cin >> cols;

    // Declaring the 2D array with the specified dimensions
    int matrix[rows][cols];

    // Asking user to input values into the 2D array
    cout << "Enter the elements of the array:" << endl;
    for (int i = 0; i < rows; i++) {
        for (int j = 0; j < cols; j++) {
            cin >> matrix[i][j];
        }
    }

    // Calculating the sum of all elements in the array
    int sum = 0;
    for (int i = 0; i < rows; i++) {
        for (int j = 0; j < cols; j++) {
            sum += matrix[i][j];
        }
    }

    // Output the sum of all elements
    cout << "The sum of all elements in the array is: " << sum << endl;

    return 0;
}
```
1. Ask User for Dimensions:
    - Prompts the user to enter the number of rows and columns for the 2D array.
```cpp
int rows, cols;
cout << "Enter the number of rows: ";
cin >> rows;
cout << "Enter the number of columns: ";
cin >> cols;
```
2. Declare the 2D Array:
    - Declares a two-dimensional array named `matrix` with the specified number of rows and columns.
```cpp
int matrix[rows][cols];
```


3. Input Values into the Array:
    - Prompts the user to input values for each element of the array using nested `for` loops.
```cpp
cout << "Enter the elements of the array:" << endl;
for (int i = 0; i < rows; i++) {
    for (int j = 0; j < cols; j++) {
        cin >> matrix[i][j];
    }
}
```

4. Calculate the Sum of All Elements:
    - Initializes `sum` to 0.
    - Uses nested `for` loops to iterate through each element of the array and adds it to `sum`.
```cpp
int sum = 0;
for (int i = 0; i < rows; i++) {
    for (int j = 0; j < cols; j++) {
        sum += matrix[i][j];
    }
}
```

5. Output the Sum:
```cpp
cout << "The sum of all elements in the array is: " << sum << endl;
```
Prints the sum of all elements in the array.

**Full Output Example:**
```cpp
Enter the number of rows: 3
Enter the number of columns: 4
Enter the elements of the array:
1 2 3 4
5 6 7 8
9 10 11 12
The sum of all elements in the array is: 78
```
## User-Interactive Array Input and Update Program in C++
```cpp
#include <iostream>
using namespace std;

int main() {
    int size;

    cout << "Enter the size of array: ";
    cin >> size;

    int arr[size];

    cout << "Enter " << size << " element for the array: " << endl;
    for (int i = 0; i < size; i++ ) {
        cout << "Index [" << i << "] : ";
        cin >> arr[i];
    } cout << "arr[" << size << "] = {";
    for (int i = 0; i < size; i++) {
        cout << arr[i];
        if (i < size - 1) {
            cout << ", ";
        }
    } cout << "}";
    cout << endl;

char choice;
do {
    int index, update;
    cout << "Do you want to update element u inputed? (y/n): "; 
    cin >> choice;

    if (choice == 'y' || choice == 'Y') {
    cout << "Enter the index[] you want to update: ";
    cin >> index;

    if (index >= 0 && index < size) {
        cout << "Enter the updated of index: ";
        cin >> update;
        arr[index] = update;
        cout << "update.COMPLETE!!.. arr[" << index << "]=" << update << endl;
    } else {
        cout << "Invalid!!..";
    }

    } else {
        cout << endl;
    }

} while (choice == 'y' || choice == 'Y') ;

cout << "FINAL. arr[" << size << "] = {";
for(int i = 0; i < size; i++) {
    cout << arr[i];
    if (i < size - 1) {
        cout << ", ";
    } 
} cout << "}";

}
```

```cpp
// This Topic is licensed under a Custom Proprietary License.
// Viewing is permitted. Copying, modifying, or distributing
// without explicit permission is prohibited.
// For permissions, contact [lauriojohnangelo@gmail.com].
```

[Lesson07>>](/Lesson07/Topic01.md)
