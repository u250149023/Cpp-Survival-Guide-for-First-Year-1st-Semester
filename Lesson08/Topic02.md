# For Loop
A for loop is a foundational control structure in programming that allows you to execute a block of code repeatedly for a specified number of times. It's particularly useful when you know in advance how many times you want to iterate. The loop's structure includes initialization, a condition to continue looping, and an update to the loop control variable.

Syntax:
```cpp
for (initialization; condition; update) {
    // Code to be executed
}
```
Let's create a unique example where we generate the first n terms of the Fibonacci sequence using a for loop:

```cpp
#include <iostream>
using namespace std;

int main() {
    int n;

    // Prompt the user to enter the number of Fibonacci terms
    cout << "How many terms of the Fibonacci sequence would you like to generate? ";
    cin >> n;

    // Ensure the input is positive
    if (n <= 0) {
        cout << "Please enter a positive number." << endl;
        return 1;
    }

    // Variables to store Fibonacci terms
    int first = 0, second = 1, next;

    // Print the first two terms
    cout << "Fibonacci sequence: " << first << " " << second << " ";

    // Generate and print the remaining terms
    for (int i = 3; i <= n; i++) {
        next = first + second;
        cout << next << " ";
        first = second;
        second = next;
    }
    cout << endl;

    return 0;
}
```
- Initialization: The loop counter int i = 3; starts at 3 because the first two Fibonacci terms are already printed.
- Condition: The loop runs as long as i <= n;, where n is the number of terms the user wants to generate.
- Update: i++ increments the loop counter after each iteration.
- Body: The loop calculates the next term in the Fibonacci sequence, prints it, and updates the variables first and second to prepare for the next iteration.

---

## Nested Loops
A nested loop is a loop inside another loop. This is useful for tasks that require repetitive processing within a repetitive processing context, such as working with multi-dimensional arrays or generating patterns.

Syntax:

```cpp
for (initialization; condition; update) {
    for (initialization; condition; update) {
        // Code to be executed
    }
}
```
Here's an example of using nested loops to print a multiplication table:

```cpp
#include <iostream>
using namespace std;

int main() {
    int n;

    // Prompt user to enter the size of the multiplication table
    cout << "Enter the size of the multiplication table: ";
    cin >> n;

    // Generate the multiplication table using nested loops
    for (int i = 1; i <= n; ++i) {
        for (int j = 1; j <= n; ++j) {
            // Print the product of i and j
            cout << i * j << "\t";
        }
        // Move to the next line after printing each row
        cout << endl;
    }

    return 0;
}
```
- Outer Loop: The outer for loop runs from 1 to n and is responsible for the rows of the multiplication table.
- Inner Loop: The inner for loop also runs from 1 to n and handles the columns of the multiplication table.
- Body: The body of the inner loop calculates and prints the product of the current row and column values (i * j), followed by a tab -character (\t) for formatting.
- New Line: After each row is printed, cout << endl; moves to the next line.

This approach creates a multiplication table of size n x n, demonstrating the power of nested loops in handling multi-level iterative tasks.
