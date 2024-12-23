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
        
