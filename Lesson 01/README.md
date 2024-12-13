## C++ Overview

**C++** is a powerful and adaptable language that evolved from **C** and was created by *Bjarne Stroustrup* in the early 1980s. Renowned for its object-oriented capabilities, **C++** is widely utilized in system programming, game development, and sophisticated software applications. This guide thoroughly explores the language, covering everything from basic syntax to advanced topics like templates and exception handling, with clear explanations and practical code examples.

## Basic Structure

**C++** program is made up of one or more functions, starting with the `main()` function. The typical structure of a **C++** program includes:

- **Header Files**: Include statements for standard library functions and classes.
- **Namespace Declaration**: Using `namespace std;` to avoid prefixing with `std::`.
- **Function Definitions**: Including the `main()` function where execution starts.
- **Statements and Expressions**: To perform operations and computations.
```cpp
#include <iostream>

using namespace std;

int main() {
    cout << "Hello, World!" << endl;
    return 0;
}
```

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

