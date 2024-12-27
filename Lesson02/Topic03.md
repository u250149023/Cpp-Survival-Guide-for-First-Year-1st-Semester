# Bitwise Operator
Bitwise operators are used to perform operations on individual bits of integer data types. These operators are essential for tasks that require direct manipulation of bits, such as low-level programming, graphics, and encryption. Here are the common bitwise operators in C++:

AND (`&`):
- Performs a bitwise AND operation between two operands. Each bit of the result is 1 if the corresponding bits of both operands are 1, otherwise, it is 0.
```cpp
int a = 5;  // In binary: 0101
int b = 3;  // In binary: 0011
int result = a & b;  // result is 1 (0001 in binary)
```

OR (`|`):
- Performs a bitwise OR operation. Each bit of the result is 1 if at least one of the corresponding bits of the operands is 1.
```cpp
int a = 5;  // In binary: 0101
int b = 3;  // In binary: 0011
int result = a | b;  // result is 7 (0111 in binary)
```

XOR (`^`):
- Performs a bitwise XOR operation. Each bit of the result is 1 if the corresponding bits of the operands are different.
```cpp
int a = 5;  // In binary: 0101
int b = 3;  // In binary: 0011
int result = a ^ b;  // result is 6 (0110 in binary)
```

NOT (`~`):
- Performs a bitwise NOT operation, which inverts all the bits of the operand.
```cpp
int a = 5;  // In binary: 0101
int result = ~a;  // result is -6 (inverts to 1010 in binary, considering 32-bit integers)
```

Left Shift (`<<`):
- Shifts the bits of the left operand to the left by the number of positions specified by the right operand. This operation fills the vacant bits with zeros.
```cpp
int a = 5;  // In binary: 0101
int result = a << 1;  // result is 10 (1010 in binary)
```

Right Shift (`>>`):
- Shifts the bits of the left operand to the right by the number of positions specified by the right operand. This operation fills the vacant bits with the sign bit (for signed integers) or zeros (for unsigned integers).
```cpp
int a = 5;  // In binary: 0101
int result = a >> 1;  // result is 2 (0010 in binary)
```

Example Program
Here’s an example program that demonstrates the use of bitwise operators:
```cpp
#include <iostream>
using namespace std;

int main() {
    int a = 5;  // In binary: 0101
    int b = 3;  // In binary: 0011

    // Bitwise AND
    int andResult = a & b;
    cout << "a & b: " << andResult << endl;  // Output: 1

    // Bitwise OR
    int orResult = a | b;
    cout << "a | b: " << orResult << endl;  // Output: 7

    // Bitwise XOR
    int xorResult = a ^ b;
    cout << "a ^ b: " << xorResult << endl;  // Output: 6

    // Bitwise NOT
    int notResult = ~a;
    cout << "~a: " << notResult << endl;  // Output: -6 (assuming 32-bit integer representation)

    // Left Shift
    int leftShiftResult = a << 1;
    cout << "a << 1: " << leftShiftResult << endl;  // Output: 10

    // Right Shift
    int rightShiftResult = a >> 1;
    cout << "a >> 1: " << rightShiftResult << endl;  // Output: 2

    return 0;
}
```

```cpp
// This Topic is licensed under a Custom Proprietary License.
// Viewing is permitted. Copying, modifying, or distributing
// without explicit permission is prohibited.
// For permissions, contact [lauriojohnangelo@gmail.com].
```

[Lesson03>>](/Lesson03/Topic01.md)



