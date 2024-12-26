# Output Operations

**Output operations** are essential in programming because they allow programs to present information to the user. In **C++** programming, output can be shown on the screen or console using the `cout` stream. This guide will explain the fundamentals of output operations in **C++**, including how to display output and use `cout` for formatted output.

## Displaying Output to the Screen/Console
In C++, **output operations** let programs show information to the user. You can display output on the screen or console using the `cout` stream. This guide covers the basics of using `cout` for output and formatting.
```cpp
#include <iostream>

int main() {
    std::cout << "Hello, World!" << std::endl; // Display "Hello, World!" on the screen
    return 0; 
}
```
The `cout` stream prints "Hello, World!" to the screen. The operator inserts data into `cout`, and `std::endl` moves to the next line.

## Using \n for Newlines

The `\n` character inserts a newline in the output, moving the cursor to the next line's start and helping to format text neatly. While `std::endl` is common, `\n` is more efficient when you don't need to flush the output buffer.
```cpp
#include <iostream>
  
int main() {
    std::cout << "First line\n";
    std::cout << "Second line\n";
    std::cout << "Third line\n";
    return 0;
}
```

## Using cout for Formatted Output

The `cout` stream in C++ allows you to format the output, like setting decimal places for numbers or adding spaces to strings. You use manipulators with `cout` to control this formatting.
```cpp
#include <iostream>
#include <iomanip>

int main() {
    int num1 = 10;
    float num2 = 3.14159;
    char letter = 'A';

    std::cout << "Integer: " << num1 << std::endl;
    std::cout << "Float: " << std::fixed << std::setprecision(2) << num2 << std::endl;
    std::cout << "Character: " << letter << std::endl;

    return 0;
}
```
In the above code, `std::fixed` and `std::setprecision(2)` are manipulators used to specify the number of decimal places for the `num2` variable. The output will display the values of the variables in the specified format.

```cpp
// This code is licensed under a Custom Proprietary License.
// Viewing is permitted. Copying, modifying, or distributing
// without explicit permission is prohibited.
// For permissions, contact [Your Contact Information].
```

[NextTopic>>](./Topic03.md)

