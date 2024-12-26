# Iterative structure
An iterative structure, or loop, is a fundamental programming concept that enables the repeated execution of a set of instructions based on a specified condition. Loops are crucial for efficiently handling tasks that involve repetitive processing, such as iterating through items in a collection, performing repetitive calculations, or building complex algorithms.

1. While Loop:
    - Executes a block of code as long as a specified condition is true.
```cpp
while (condition) {
    // Code to be executed
}
```
2. For Loop:
    - Executes a block of code a specific number of times.
```cpp
for (initialization; condition; increment) {
    // Code to be executed
}
```
3. Do-While Loop:
    - Similar to a while loop, but the condition is checked after the code block is executed, ensuring that the code is executed at least once.
```cpp
do {
    // Code to be executed
} while (condition);
```

---

```cpp
#include <iostream>
using namespace std;

int main() {
    // While loop example
    int count = 0;
    while (count < 5) {
        cout << "While loop count: " << count << endl;
        count++;
    }

    // For loop example
    for (int i = 0; i < 5; i++) {
        cout << "For loop iteration: " << i << endl;
    }

    // Do-While loop example
    int num = 0;
    do {
        cout << "Do-While loop number: " << num << endl;
        num++;
    } while (num < 5);

    return 0;
}
```
- The while loop executes as long as count is less than 5.
- The for loop iterates 5 times, from 0 to 4.
- The do-while loop executes at least once and continues as long as num is less than 5.

Iterative structures are powerful tools in programming, enabling you to perform repetitive tasks efficiently and effectively.

---

## While Loop
A while loop is a control flow statement that allows code to be executed repeatedly based on a given boolean condition. The while loop continues to execute as long as the condition remains true. If the condition evaluates to false, the loop terminates and the control passes to the next statement after the loop.

``` cpp
#include <iostream>
using namespace std;

int main() {
    int n;
    cout << "Enter a number to calculate its factorial: ";
    cin >> n;

    int factorial = 1;
    int i = n;

    while (i > 1) {
        factorial *= i; // Multiply current factorial by i
        i--;            // Decrement i
    }

    cout << "The factorial of " << n << " is " << factorial << endl;
    return 0;
}
```

## Do-While Loop
A do-while loop is similar to a while loop, except that the condition is evaluated after the execution of the loop's body. This means that the code inside the do-while loop will always execute at least once, regardless of whether the condition is true or false.

```cpp
#include <iostream>
using namespace std;

int main() {
    int num;

    do {
        cout << "Enter a positive number: ";
        cin >> num;

        if (num <= 0) {
            cout << "Invalid input. Please try again." << endl;
        }
    } while (num <= 0);

    cout << "You entered a positive number: " << num << endl;
    return 0;
}
```

The while loop calculates the factorial of a given number.
The do-while loop ensures the user enters a positive number by repeating the prompt until a valid input is provided.

```cpp
// This Topic is licensed under a Custom Proprietary License.
// Viewing is permitted. Copying, modifying, or distributing
// without explicit permission is prohibited.
// For permissions, contact [lauriojohnangelo@gmail.com].
```
