# One Dimensional Arrays
A one-dimensional array, often referred to simply as an array, is a data structure that stores a collection of elements of the same type in a single, linear sequence. Think of it as a list of items where each item can be accessed by its position or index in the list.

## Creating, Traversing, and Modifying a One-Dimensional Array in C++
```cpp
#include <iostream>
using namespace std;

int main() {
    // Declaration and Initialization
    int numbers[5] = {1, 2, 3, 4, 5}; // Declares and initializes an array with 5 elements

    // Accessing and Modifying Elements
    cout << "The third element is: " << numbers[2] << endl; // Accesses and prints the third element (index 2)

    numbers[2] = 10; // Modifies the third element to 10
    cout << "The third element after modification is: " << numbers[2] << endl; // Prints the modified third element

    // Looping through the array
    cout << "All elements in the array: ";
    for (int i = 0; i < 5; i++) {
        cout << numbers[i] << " "; // Prints each element of the array
    }
    cout << endl; // Moves to the next line after printing all elements

    return 0; // Ends the program
}
```
1. Array Declaration and Initialization:
   - Declares an array named `numbers` with 5 integer elements and initializes them with values `{1, 2, 3, 4, 5}`.
3. Accessing and Modifying Elements:
   - `cout << "The third element is: " << numbers[2] << endl;`: Accesses and prints the third element of the array (index 2), which is `3`.
   - `numbers[2] = 10;`: Modifies the third element of the array to `10`.
   - `cout << "The third element after modification is: " << numbers[2] << endl;`: Prints the modified third element, which is now `10`.
5. Looping through the Array:
   - `cout << "All elements in the array: ";`: Prints a message before displaying all elements.
   - `for (int i = 0; i < 5; i++) { ... }`: Uses a `for` loop to iterate through each element of the array.
   - `cout << numbers[i] << " ";`: Prints each element of the array, separated by a space.
   - `cout << endl;`: Moves to the next line after printing all elements.

   This code demonstrates how to declare, initialize, access, modify, and loop through a one-dimensional array in C++
