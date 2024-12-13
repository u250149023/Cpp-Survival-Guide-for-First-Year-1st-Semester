## Output Operations

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
