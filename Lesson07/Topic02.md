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
