# Boolean Operators
Boolean operators, also known as logical operators, are used in programming to perform logical operations on boolean values (true or false). These operators allow you to combine multiple conditions or invert conditions to make more complex logical decisions.

Common Boolean Operators:

AND (`&&`):
Returns true if both operands are true.
```cpp
bool result = (condition1 && condition2);
```

OR (`||`):
Returns true if at least one of the operands is true.
```cpp
bool result = (condition1 || condition2);
```

NOT (`!`):
Returns the opposite boolean value of its operand (true becomes false, and false becomes true).
```cpp
bool result = !condition;
```

Example:

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

AND (`&&`): Combines two conditions and returns true only if both are true. Otherwise, it returns false.
OR (`||`): Combines two conditions and returns true if at least one of them is true. If both are false, it returns false.
NOT (`!`): Inverts the boolean value of a condition. If the condition is true, ! makes it false, and vice versa.

Boolean operators are essential for making complex logical decisions in programming, enabling you to build more sophisticated conditions and control the flow of your program effectively.

