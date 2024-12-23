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

## Using User Input and Logical Operators
```cpp
#include <iostream>
using namespace std;

int main() {
    int age;
    char permission;
    char membership;

    // Get user input for age
    cout << "Enter your age: ";
    cin >> age;

    // Get user input for permission
    cout << "Do you have permission? (y/n): ";
    cin >> permission;

    // Get user input for membership
    cout << "Do you have a membership? (y/n): ";
    cin >> membership;

    // Outer condition: Check if age is greater than or equal to 18
    if (age >= 18) {
        // Nested condition with logical operators
        if ((permission == 'y' || permission == 'Y') && (membership == 'y' || membership == 'Y')) {
            cout << "You are allowed to enter the event." << endl;
        } else if ((permission == 'y' || permission == 'Y') && !(membership == 'y' || membership == 'Y')) {
            cout << "You need a membership to enter the event." << endl;
        } else {
            cout << "You need permission to enter the event." << endl;
        }
    } else {
        // Using != operator and less than
        if (age != 0 && age < 18) {
            cout << "You are not old enough to enter the event." << endl;
        } else {
            cout << "Invalid age input." << endl;
        }
    }

    return 0;
}
```
- **Input**: cin is used to get the user's age, permission status, and membership status.
- **Outer Condition**: if (age >= 18) checks if the user's age is 18 or older.
- **Nested Conditions with Logical Operators**:
    - && (and): Ensures both conditions are true.
    - || (or): Ensures at least one condition is true.
    - ! (not): Inverts the condition.

- **Comparison Operators**:
    - == (equal to): Checks if two values are equal.
    - != (not equal to): Checks if two values are not equal.
    - > (greater than) and < (less than): Compare numerical values.

This structure demonstrates how to use nested decisions with various logical and comparison operators.
