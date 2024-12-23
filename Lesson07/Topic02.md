# IF, ELSE IF AND ELSE 
"if", "else if", and "else" statements work similarly to other programming languages by controlling the flow of the program based on specific conditions. The "if" statement checks a condition, and if it's true, executes a particular block of code. "else if" checks additional conditions if the previous "if" or "else if" conditions are false. Finally, "else" handles any cases not covered by the preceding conditions.
```cpp
#include <iostream> 
using namespace std; 

int main() {
    int age; // Variable to store user's age

    cout << "Enter your age: "; // Prompt user for age
    cin >> age; // Read user input

    if (age < 13) { // Check if age is less than 13
        cout << "You are a child." << endl; // Age less than 13
    } else if (age < 20) { // Check if age is less than 20
        cout << "You are a teenager." << endl; // Age between 13 and 19
    } else if (age < 65) { // Check if age is less than 65
        cout << "You are an adult." << endl; // Age between 20 and 64
    } else { // Age 65 or older
        cout << "You are a senior." << endl; // Age 65 or older
    }

    return 0; 
}
```

---
# SWITCH STATEMENT
A `switch` statement in C++ is a control flow statement that allows you to execute one of many possible code blocks based on the value of a single variable or expression. It's a more streamlined way to handle multiple conditional paths compared to multiple `if-else` if statements. The `switch` statement evaluates an expression and matches its value to a case label, executing the corresponding code block. If no match is found, it can optionally execute a `default` case.

## Syntax of a Switch Statement
```cpp
switch (expression) {
    case constant1:
        // code block
        break;
    case constant2:
        // code block
        break;
    // additional cases as needed
    default:
        // code block if no case matches
}
```
## Example
```cpp
#include <iostream>
using namespace std;

int main() {
    int day = 3;

    switch (day) {
        case 1:
            cout << "Monday" << endl;
            break;
        case 2:
            cout << "Tuesday" << endl;
            break;
        case 3:
            cout << "Wednesday" << endl;
            break;
        case 4:
            cout << "Thursday" << endl;
            break;
        case 5:
            cout << "Friday" << endl;
            break;
        case 6:
            cout << "Saturday" << endl;
            break;
        case 7:
            cout << "Sunday" << endl;
            break;
        default:
            cout << "Invalid day" << endl;
    }

    return 0;
}
```

1. Variable Declaration and Initialization:
    - Declares an integer variable day and initializes it with the value 3.
```cpp
int day = 3;
```


2. Switch Statement:
    - Starts the switch statement, which will evaluate the value of the variable day.
```cpp
switch (day) {
```

3. Case Statements:
    - Each case statement checks if day matches a constant value. If a match is found, the corresponding code block is executed. The `break` statement exits the switch after executing the matched case's block to prevent "fall-through" to subsequent cases.
```cpp
case 1:
    cout << "Monday" << endl;
    break;
case 2:
    cout << "Tuesday" << endl;
    break;
case 3:
    cout << "Wednesday" << endl;
    break;
// Additional cases for other days
```

4. Default Case:
    - If no matching case is found, the `default` case is executed. It's an optional part of the switch statement that handles unexpected values.
```cpp
default:
    cout << "Invalid day" << endl;
```

This approach can make the code more readable and manageable, especially when dealing with multiple discrete values.
