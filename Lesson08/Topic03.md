# Break
The break statement is a powerful control mechanism in C++ that allows you to exit a loop or switch statement before it has completed all its iterations or cases. This is especially useful when you need to terminate a loop based on a specific condition.

Syntax:

```cpp
for (initialization; condition; update) {
    if (some_condition) {
        break;  // Exit the loop
    }
    // Other code
}
```

```cpp
#include <iostream>
using namespace std;

int main() {
    int threshold;
    cout << "Enter the threshold value to stop: ";
    cin >> threshold;

    cout << "Keep entering numbers. I'll stop if a number exceeds the threshold of " << threshold << "." << endl;

    int number;
    while (true) {
        cin >> number;
        
        if (number > threshold) {
            cout << "Number " << number << " exceeds the threshold of " << threshold << ". Exiting loop." << endl;
            break;  // Exit the loop if the number exceeds the threshold
        }

        cout << "You entered: " << number << ". Keep going or enter a number greater than " << threshold << " to stop." << endl;
    }

    cout << "Loop ended as a number exceeding the threshold was entered." << endl;

    return 0;
}
```
- Threshold Input: The program first asks the user to enter a threshold value. If a number exceeds this value, the loop will terminate.
- Infinite Loop: while (true) creates a loop that runs indefinitely until the break statement is encountered.
- User Input: The program continuously reads numbers entered by the user.
- Condition Check: The loop checks if the entered number exceeds the threshold. If it does, the break statement is executed to exit the loop.
- Output: The program provides feedback on each number entered and informs the user that entering a number greater than the threshold will stop the loop.

This example uniquely demonstrates how the break statement can be used to control the flow of a loop based on user-defined criteria.

---
 
# Continue
The continue statement in C++ is used to skip the remaining part of the loop and start the next iteration. This is particularly useful when you want to bypass certain parts of the loop based on a condition without exiting the loop entirely.

```cpp
for (initialization; condition; update) {
    if (some_condition) {
        continue;  // Skip to the next iteration
    }
    // Other code
}
```

```cpp
#include <iostream>
using namespace std;

int main() {
    int number;
    int sum = 0;

    cout << "Enter numbers to sum (enter 0 to stop): ";

    while (true) {
        cin >> number;

        if (number == 0) {
            break;  // Exit the loop if the user enters 0
        }

        if (number < 0) {
            cout << "Skipping negative number: " << number << endl;
            continue;  // Skip this iteration if the number is negative
        }

        sum += number;  // Add positive number to sum
    }

    cout << "The sum of positive numbers entered is: " << sum << endl;

    return 0;
}
```

- Infinite Loop: while (true) creates a loop that runs indefinitely until the break statement is encountered.
User Input: The program continuously reads numbers entered by the user.
- Exit Condition: If the user enters 0, the loop exits using break.
- Skip Condition: If the number is negative, a message is printed, and the continue statement skips the rest of the loop body, starting the next iteration.
- Summation: If the number is positive, it is added to the running total sum.

This approach highlights how the continue statement can be used to control the flow of a loop by selectively skipping certain iterations based on conditions.

```cpp
// This Topic is licensed under a Custom Proprietary License.
// Viewing is permitted. Copying, modifying, or distributing
// without explicit permission is prohibited.
// For permissions, contact [lauriojohnangelo@gmail.com].
```
