# Assignment Operators
The assignment operator in C++ is used to assign values to variables. The most common assignment operator is the equal sign (=), which assigns the value on the right to the variable on the left. In addition to the basic assignment operator, there are compound assignment operators that combine an arithmetic operation with assignment.

## Basic Assignment Operator (`=`):
The basic assignment operator is used to assign a value to a variable.
Example:
```cpp
#include <iostream>
using namespace std;

int main() {
    int x;  // Declare an integer variable
    x = 10;  // Assign the value 10 to the variable x
    cout << "The value of x is: " << x << endl;  // Output the value of x
    return 0;
}
```

## Compound Assignment Operators
Compound assignment operators perform an arithmetic operation and assign the result to the variable. Here are some common compound assignment operators:

Addition Assignment (`+=`):
Adds the right operand to the left operand and assigns the result to the left operand.
```cpp
int a = 5;
a += 3;  // Equivalent to a = a + 3; a is now 8
```

Subtraction Assignment (`-=`):
Subtracts the right operand from the left operand and assigns the result to the left operand.
```cpp
int b = 5;
b -= 2;  // Equivalent to b = b - 2; b is now 3
```

Multiplication Assignment (`*=`):
Multiplies the left operand by the right operand and assigns the result to the left operand.
```cpp
int c = 4;
c *= 2;  // Equivalent to c = c * 2; c is now 8
```

Division Assignment (`/=`):
Divides the left operand by the right operand and assigns the result to the left operand.
```cpp
int d = 10;
d /= 2;  // Equivalent to d = d / 2; d is now 5
```

Modulus Assignment (`%=`):
Takes the modulus of the left operand by the right operand and assigns the result to the left operand.
```cpp
int e = 10;
e %= 3;  // Equivalent to e = e % 3; e is now 1
```

Example Program
Here’s an example program that demonstrates the use of both basic and compound assignment operators:
```cpp
#include <iostream>
using namespace std;

int main() {
    int x = 10;
    int y = 5;

    // Basic assignment
    x = y;
    cout << "x = y: x = " << x << endl;

    // Compound assignment operators
    x += 2;
    cout << "x += 2: x = " << x << endl;

    x -= 1;
    cout << "x -= 1: x = " << x << endl;

    x *= 3;
    cout << "x *= 3: x = " << x << endl;

    x /= 2;
    cout << "x /= 2: x = " << x << endl;

    x %= 3;
    cout << "x %= 3: x = " << x << endl;

    return 0
```

```cpp
// This Topic is licensed under a Custom Proprietary License.
// Viewing is permitted. Copying, modifying, or distributing
// without explicit permission is prohibited.
// For permissions, contact [lauriojohnangelo@gmail.com].
```

[NextTopic>>](./Topic03.md)
