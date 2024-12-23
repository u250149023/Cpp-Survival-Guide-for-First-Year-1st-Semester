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


