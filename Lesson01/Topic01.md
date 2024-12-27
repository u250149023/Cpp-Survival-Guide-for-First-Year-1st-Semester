# Overview of C++
C++ is a robust and versatile programming language designed to bridge the gap between high-level and low-level programming. Developed by **Bjarne Stroustrup** in the early 1980s, it extends the C language with object-oriented features, enabling efficient and modular code development. Here are the key highlights:

- **Object-Oriented Programming**: C++ incorporates classes, inheritance, polymorphism, and encapsulation, which promote code reuse     and simplify complex software projects.
- **Standard Template Library (STL)**: The STL provides a rich set of template classes and functions for data structures and algorithms, making it easy to implement common tasks without reinventing the wheel.
- **Memory Management**: With pointers and dynamic memory allocation, C++ offers fine-grained control over memory, though it requires careful handling to avoid errors.
- **Performance**: Known for its efficiency, C++ is ideal for applications demanding real-time processing, such as games and operating systems.
- **Compatibility with C**: It maintains compatibility with C, allowing seamless integration of existing C code and libraries.
- **Templates and Generics**: Templates enable the creation of functions and classes that work with any data type, enhancing code flexibility and reuse.
- **Exception Handling**: C++ supports structured error handling, making programs more robust and easier to debug.
- **Rich Library Ecosystem**: Beyond the STL, C++ has extensive libraries for networking, threading, graphics, and more, catering to diverse application needs.

## Basic Structure of a C++ Program
The basic structure of a C++ program consists of several key components that form the foundation of any C++ application. Understanding these components is essential for writing functional and well-organized code.

The basic structure of a C++ program refers to the essential elements and the layout of the code, which includes:
    - **Preprocessor Directives**: Commands that instruct the compiler to process certain files before compiling the program, such as including libraries.
    - **Namespace Declaration**: Used to avoid naming conflicts by grouping entities under a common name.
    - **Main Function**: The entry point of every C++ program, where execution starts.
    - **Variable Declarations**: Defining variables that will be used in the program.
    - **Statements and Expressions**: The logic and behavior of the program contained within the main function.
    - **Return Statement**: Indicates the end of the main function and returns a value to the operating system.
```cpp
#include <iostream>  // Include necessary library

using namespace std; // Use standard namespace

int main() {
    int number = 42; // Declare and initialize a variable
    cout << "The number is: " << number << endl; // Output the variable's value
    return 0; // End the program
}
```
- **Preprocessor Directive**: `#include <iostream>` includes the iostream library for input and output operations.
- **Namespace Declaration**: `using namespace std;` allows the use of standard library names without prefixing them with `std::`.
- **Main Function**: `int main(` is the starting point of the program.
- **Variable Declarations**: `int number = 42;` defines an integer variable and assigns it a value.
- **Statements and Expressions**: `cout << "The number is: " << number << endl;` prints the value of the variable to the console.
- **Return Statement**: `return 0;` ends the main function and returns 0 to indicate successful execution.

## Headers 

In **C++**, header files are used to declare functions and classes. The standard library headers generally do not have a `.h` extension. Some frequently used headers are:

- `<iostream>`: For standard input and output stream objects like cin and cout.
- `<vector>`: For using the vector container.
- `<string>`: To use the string class.
- `<algorithm>`: For common algorithms like sort, search, etc.
- `<cmath>`: For mathematical functions.
```cpp
1	#include <iostream>  // Standard I/O
2	#include <vector>    // Vector container
3	// Other headers...
```
## Syntax Rules
**Syntax** rules in programming refer to the guidelines and conventions that determine the structure of a valid program. These rules ensure that the code is properly formatted and can be interpreted correctly by the compiler or interpreter.

**C++** syntax is derived from **C** and includes the following:

- **Case Sensitivity**: C++ distinguishes between uppercase and lowercase letters.
- **Semicolons**: Every statement must end with a semicolon.
- **Braces**: Braces define the scope of functions and control structures.
```cpp
1	int main() {
2	    int a = 5;
3	    a++;
4	    cout << a;  // Outputs 6
5	    return 0;
6	}
```
## Comments
**Comments** in programming are annotations that explain the code, making it easier for developers to understand and maintain. They are ignored by the compiler and do not affect the program's execution.

- **Single-Line** Comments: Begin with `//` and continue to the end of the line.
- **Multi-Line** Comments: Enclosed between `/*` and `*/`, can span multiple lines.
```cpp
1	// This is a single-line comment
2	/* This is a
3	   multi-line comment */
```

## Variables
**Variables** are essential storage units in C++ programming. Here are the rules for naming variables:
- **Start with a Letter or Underscore**: Variable names must begin with a letter (A-Z or a-z) or an underscore (_).
- **Alphanumeric and Underscores**: Variable names can include letters, digits, and underscores.
- **Avoid Reserved Keywords**: Reserved words in C++ (such as `class`, `void`, `int`, etc.) cannot be used as variable names.
- **Case Sensitivity**: C++ is case-sensitive, meaning `Variable`, `variable`, and `VARIABLE` are considered different.
```cpp
1	int mainCount;
2	float totalPrice;
3	bool isValid;
```

## Data Types
**Data types** define the kind of data that can be stored and manipulated within a program. **C++** supports a variety of data types:
- **Basic Data Types**: These include `int` (integer), `char` (character), `float` (floating-point), and `double` (double precision floating-point).
- **Derived Data Types**: These include `arrays` (collections of elements), `pointers` (variables that store memory addresses), and user-defined types such as `classes`.

## Constant 
**Constants** are fixed values that do not change during the execution of a program. They are used to define data that remains the same, providing a way to protect critical values from being altered.

- **Literals**: Directly assigned constant values like `42`, `'A'`, `3.14`, `"Hello, World!"`.
- **const Keyword**: Used to declare `constants`. Once a value is assigned, it cannot be changed.
```cpp
1	const int MAX_SIZE = 100;
```
## Reserved Words
**Reserved words** (also known as keywords) are predefined words in **C++** that have special meaning to the compiler. These words cannot be used as identifiers (such as **variable names**, **function names**, etc.) because they are part of the **C++ syntax**.

- **Data Types**: `int`, `char`, `float`, `double`, `void`, `bool`
- **Control Structures**: `if`, `else`, `switch`, `case`, `for`, `while`, `do`, `break`, `continue`
- **Access Specifiers**: `public`, `private`, `protected`
- **Class Related**: `class`, `struct`, `union`, `enum`, `new`, `delete`, `this`
- **Other Keywords**: `return`, `const`, `static`, `extern`, `register`, `sizeof`, `typedef`, `namespace`, `using`

```cpp
// This Topic is licensed under a Custom Proprietary License.
// Viewing is permitted. Copying, modifying, or distributing
// without explicit permission is prohibited.
// For permissions, contact [lauriojohnangelo@gmail.com].
```
  
  [NextTopic>>](./Topic02.md)
