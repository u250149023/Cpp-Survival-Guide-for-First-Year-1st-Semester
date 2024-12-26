# Selection Structure
A selection structure, also known as a decision structure, is a fundamental concept in programming that allows a program to choose different paths of execution based on certain conditions. It enables the program to make decisions and execute specific blocks of code depending on whether a condition is true or false.

## Conditional Statements
Conditional statements, also known as decision-making statements, are fundamental constructs in programming that allow the execution of different blocks of code based on whether a specified condition is true or false. These statements enable programs to make decisions and execute different code paths depending on various conditions.

### Types of Conditional Statements:
- If Statement:
  - Executes a block of code if a specified condition is true.
```cpp
if (condition) {
    // Code to execute if condition is true
}
```

- If-Else Statement:
  - Executes one block of code if a condition is true and another block if the condition is false.
```cpp
if (condition) {
    // Code to execute if condition is true
} else {
    // Code to execute if condition is false
}
```

- If-Else If-Else Statement:
  - Evaluates multiple conditions and executes the corresponding block of code for the first true condition. If none of the conditions are true, the else block is executed.
```cpp
if (condition1) {
    // Code to execute if condition1 is true
} else if (condition2) {
    // Code to execute if condition2 is true
} else {
    // Code to execute if none of the conditions are true
}
```

- Switch Statement:
  - Evaluates an expression and executes the corresponding case block. It's typically used when you have multiple possible values for a single variable.
```cpp
switch (expression) {
    case value1:
        // Code to execute if expression is equal to value1
        break;
    case value2:
        // Code to execute if expression is equal to value2
        break;
    default:
```

---

# Relational Operators
Relational operators are used in programming to compare two values or expressions. These operators evaluate the relationship between the operands and return a boolean value: true if the relationship holds, and false otherwise. Relational operators are fundamental for making decisions and controlling the flow of a program.

Common Relational Operators:

Equal To (==):
Checks if two values are equal.
```cpp
int a = 5;
int b = 5;
bool result = (a == b); // result is true
```

Not Equal To (!=):
Checks if two values are not equal.
```cpp
int a = 5;
int b = 6;
bool result = (a != b); // result is true
```

Greater Than (>):
Checks if the value on the left is greater than the value on the right.
```cpp
int a = 7;
int b = 5;
bool result = (a > b); // result is true
```

Less Than (<):
Checks if the value on the left is less than the value on the right.
```cpp
int a = 3;
int b = 5;
bool result = (a < b); // result is true
```

Greater Than or Equal To (>=):
Checks if the value on the left is greater than or equal to the value on the right.
```cpp
int a = 5;
int b = 5;
bool result = (a >= b); // result is true
```

Less Than or Equal To (<=):
Checks if the value on the left is less than or equal to the value on the right.
```cpp
int a = 4;
int b = 5;
bool result = (a <= b); // result is true
```

---

# Boolean Operators
Boolean operators, also known as logical operators, are used in programming to perform logical operations on boolean values (true or false). These operators allow you to combine multiple conditions or invert conditions to make more complex logical decisions.

## Common Boolean Operators:

- AND (`&&`):
Returns true if both operands are true.
```cpp
bool result = (condition1 && condition2);
```

- OR (`||`):
Returns true if at least one of the operands is true.
```cpp
bool result = (condition1 || condition2);
```

- NOT (`!`):
Returns the opposite boolean value of its operand (true becomes false, and false becomes true).
```cpp
bool result = !condition;
```

### Example:
AND Operator Example:
```cpp
#include <iostream>
using namespace std;

int main() {
    int a = 10;
    int b = 20;
    bool result = (a > 5 && b > 15); // Both conditions are true

    if (result) {
        cout << "Both conditions are true." << endl;
    } else {
        cout << "One or both conditions are false." << endl;
    }

    return 0;
}
```

OR Operator Example:
```cpp
#include <iostream>
using namespace std;

int main() {
    int a = 10;
    int b = 5;
    bool result = (a > 5 || b > 15); // At least one condition is true

    if (result) {
        cout << "At least one condition is true." << endl;
    } else {
        cout << "Both conditions are false." << endl;
    }

    return 0;
}
```

NOT Operator Example:
```cpp
#include <iostream>
using namespace std;

int main() {
    int a = 10;
    bool result = !(a > 5); // Inverting the condition

    if (result) {
        cout << "The condition is false." << endl;
    } else {
        cout << "The condition is true." << endl;
    }

    return 0;
}
```

- AND (`&&`): Combines two conditions and returns true only if both are true. Otherwise, it returns false.
- OR (`||`): Combines two conditions and returns true if at least one of them is true. If both are false, it returns false.
- NOT (`!`): Inverts the boolean value of a condition. If the condition is true, ! makes it false, and vice versa.



## Short-Circuit Evaluation
Short-circuit evaluation is a feature in many programming languages where the second operand in a logical operation is evaluated only if the first operand is not sufficient to determine the result of the operation. This mechanism is commonly used with the logical operators && (AND) and || (OR).

Here's an example where short-circuit evaluation can prevent potential runtime errors, such as division by zero:
```cpp
#include <iostream>
using namespace std;

int main() {
    int x = 0;
    int y = 10;

    if (x != 0 && (y / x) > 2) {
        cout << "This will not execute." << endl;
    } else {
        cout << "Short-circuit evaluation prevents division by zero." << endl;
    }

    return 0;
}
```
- In this example, the division y / x is not executed because the first condition x != 0 is false. Thus, it prevents a potential division-by-zero error.
Short-circuit evaluation is a powerful feature that can make your code more efficient and safer by avoiding unnecessary computations and potential errors.

Boolean operators are essential for making complex logical decisions in programming, enabling you to build more sophisticated conditions and control the flow of your program effectively.

```cpp
// This Topic is licensed under a Custom Proprietary License.
// Viewing is permitted. Copying, modifying, or distributing
// without explicit permission is prohibited.
// For permissions, contact [lauriojohnangelo@gmail.com].
```

[NextTopic>>](./Topic01.md)
