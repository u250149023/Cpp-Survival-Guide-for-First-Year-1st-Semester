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

