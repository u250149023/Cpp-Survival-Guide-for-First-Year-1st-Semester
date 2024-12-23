# NESTED DECISION
A nested decision in C++ refers to placing one `if` statement inside another `if` statement. This allows for evaluating multiple conditions in a hierarchical manner, enabling more complex decision-making processes.

1. **Outer Condition**: The first `if` statement checks an initial condition.
2. **Nested Condition**: Inside the outer `if` statement, another `if` statement checks an additional condition.
3. **Actions**: Different actions are taken based on the outcome of the nested conditions.

```cpp
#include <iostream>
using namespace std;

int main() {
    int age = 20;
    bool hasPermission = true;

    // Outer condition: Check if age is greater than or equal to 18
    if (age >= 18) {
        // Nested condition: Check if the person has permission
        if (hasPermission) {
            cout << "You are allowed to enter the event." << endl;
        } else {
            cout << "You need permission to enter the event." << endl;
        }
    } else {
        cout << "You are not old enough to enter the event." << endl;
    }

    return 0;
}
```
In this example:
1. Outer Condition: `if (age >= 18)` checks if the person's age is 18 or older.
2. Nested Condition: Inside the first `if`, `if (hasPermission)` checks if the person has permission.
3. Actions: Different messages are printed based on the conditions.

Nested decisions allow for more detailed and layered decision-making, making it easier to handle complex logic in your programs.
