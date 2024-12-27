# Arithmetic Operators
Arithmetic operators are used to perform basic mathematical operations on numeric data types. Here are the most common arithmetic operators in C++:

Addition (`+`):
Adds two operands.
```cpp
int a = 5, b = 3;
int sum = a + b;  // sum = 8
```

Subtraction (`-`):
Subtracts the second operand from the first.
```cpp
int a = 5, b = 3;
int difference = a - b;  // difference = 2
```

Multiplication (`*`):
Multiplies two operands.
```cpp
int a = 5, b = 3;
int product = a * b;  // product = 15
```

Division (`/`):
Divides the first operand by the second. If both operands are integers, the result is an integer.
```cpp
int a = 6, b = 3;
int quotient = a / b;  // quotient = 2

double x = 5.0, y = 2.0;
double quotient2 = x / y;  // quotient2 = 2.5
```

Modulus (`%`):
Returns the remainder of a division operation. It only works with integers.
```cpp
int a = 5, b = 3;
int remainder = a % b;  // remainder = 2
```

Here’s an example program that demonstrates the use of these arithmetic operators:

```cpp
#include <iostream>
using namespace std;

int main() {
    int a = 10;
    int b = 3;

    // Addition
    int sum = a + b;
    cout << "Sum: " << sum << endl;

    // Subtraction
    int difference = a - b;
    cout << "Difference: " << difference << endl;

    // Multiplication
    int product = a * b;
    cout << "Product: " << product << endl;

    // Division
    int quotient = a / b;
    cout << "Quotient: " << quotient << endl;

    // Modulus
    int remainder = a % b;
    cout << "Remainder: " << remainder << endl;

    return 0
```


```cpp
// This Topic is licensed under a Custom Proprietary License.
// Viewing is permitted. Copying, modifying, or distributing
// without explicit permission is prohibited.
// For permissions, contact [lauriojohnangelo@gmail.com].
```

[NextTopic>>](./Topic02.md)
