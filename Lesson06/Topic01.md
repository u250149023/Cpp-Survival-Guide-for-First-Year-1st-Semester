# Array
An **array** is a fundamental data structure in programming that allows you to store a collection of elements of the same type in a contiguous block of memory. Think of it as a list of items, like a row of lockers, where each locker (or array element) holds a value, and you can access each one using an index or position.

## Key Features of Arrays:
- **Fixed Size**: Once you declare an array, its size is fixed and cannot be changed. You need to specify the number of elements (size) when you create the array.

- **Indexing**: Elements in an array are accessed using an index, which usually starts from 0. For example, the first element is at index 0, the second element at index 1, and so on.

- **Homogeneous Elements**: All elements in an array are of the same type. If you declare an array of integers, all elements must be integers.

- **Contiguous Memory Allocation**: The elements of an array are stored in contiguous memory locations, allowing for efficient access and manipulation.


## Declaration, Initialization, and Accessing Array Elements

### Declaration
```cpp
// Declare an array of a specified type and size
type arrayName[arraySize];
```
- `type`: The data type of the array elements (e.g., `int`, `float`, `char`).
- `arrayName`: The name of the array.
- `arraySize`: The number of elements the array can hold.

### Initialization
```cpp
// Initialize an integer array with 5 elements
int numbers[5] = {1, 2, 3, 4, 5};
```
- Declares and initializes an integer array named `numbers` with 5 elements: `1, 2, 3, 4, 5`

### Accessing Array Elements
```cpp
// Access an element of the array using its index
arrayName[index];
```
- Accesses an element of the array using its index. Indices start from 0.

- Example of Accessing an Array Element
```cpp
// Accessing the third element of the 'numbers' array
int value = numbers[2];  // 'value' will be 3
```
- `numbers[2]` accesses the element at index 2 of the `numbers` array, which is `3`. The value `3` is then assigned to the `variable` value.

---
## TIPS
1. Avoid Out-of-Bounds Access
- Tip: Always ensure you are accessing valid indices within the array bounds to avoid undefined behavior.
- Common Mistake: Accessing an index that is outside the array's declared size.

```cpp
int arr[5] = {1, 2, 3, 4, 5};
cout << arr[5]; // Out of bounds, valid indices are 0 to 4
```

2. Proper Initialization
- Tip: Initialize arrays to avoid unexpected values, especially if declaring an array without initial values.
- Common Mistake: Forgetting to initialize an array, which can lead to unpredictable behavior due to garbage values.

```cpp
int arr[5]; // Uninitialized array, contains garbage values
int arrInitialized[5] = {0}; // Proper initialization, all elements set to 0
```
3. Using Loops for Processing
- Tip: Use loops to efficiently traverse and process array elements.
- Common Mistake: Incorrect loop bounds, leading to out-of-bounds access or missing elements.

```cpp
int arr[5] = {1, 2, 3, 4, 5};
for (int i = 0; i < 5; ++i) { // Correct loop bounds
    cout << arr[i]
```
