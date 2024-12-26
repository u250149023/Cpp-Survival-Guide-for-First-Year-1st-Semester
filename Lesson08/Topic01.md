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
