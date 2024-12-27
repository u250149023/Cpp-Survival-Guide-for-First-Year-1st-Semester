# Typecasting 
Typecasting, also known as type conversion, is the process of converting a variable from one data type to another. In C++, typecasting can be done in two main ways: implicit (automatic) and explicit (manual). Understanding typecasting is essential for ensuring that your program handles data correctly and avoids unexpected behavior.

## Implicit Typecasting
Implicit typecasting occurs automatically when the compiler converts one data type to another. This usually happens when assigning a value of one type to a variable of another type, or when performing arithmetic operations involving different types.

```cpp
#include <iostream>
using namespace std;

int main() {
    int a = 42;
    double b = a;  // Implicit typecasting from int to double
    cout << "a (int): " << a << endl;
    cout << "b (double): " << b << endl;
    return 0;
}
```

## Explicit Typecasting
Explicit typecasting, also known as casting, is when the programmer explicitly converts a variable from one type to another using casting operators. There are several ways to perform explicit typecasting in C++:

**C-Style Cast**:
```cpp
int a = 42;
double b = (double)a;  // Explicit typecasting from int to double
```

**Function-Style Cast**:
```cpp
int a = 42;
double b = double(a);  // Explicit typecasting from int to double
```

**Static Cast**:
```cpp
int a = 42;
double b = static_cast<double>(a);  // Explicit typecasting using static_cast
```

Here’s an example program demonstrating different types of typecasting:

```cpp
#include <iostream>
using namespace std;

int main() {
    int a = 42;
    double b;

    // Implicit typecasting
    b = a;
    cout << "Implicit typecasting (int to double): " << b << endl;

    // C-Style Cast
    b = (double)a;
    cout << "C-Style Cast (int to double): " << b << endl;

    // Function-Style Cast
    b = double(a);
    cout << "Function-Style Cast (int to double): " << b << endl;

    // Static Cast
    b = static_cast<double>(a);
    cout << "Static Cast (int to double): " << b << endl;

    // Typecasting double to int
    double pi = 3.14159;
    int c = static_cast<int>(pi);  // Truncates the decimal part
    cout << "Static Cast (double to int): " << c << endl;

    return 0;
}
```
Explanation
- **Implicit Typecasting**: The compiler automatically converts the `int` variable `a` to `double` when assigning it to `b`.
- **C-Style Cast**: Uses parentheses and the target type to cast `a` to `double`.
- **Function-Style Cast**: Uses the target type as a function call to cast `a` to `double`.
- **Static Cast**: Uses the `static_cast` operator to explicitly cast `a` to `double`.
- **Typecasting from `double` to `int`**: Converts the `double` variable `pi` to `int`, truncating the decimal part.

```cpp
// This Topic is licensed under a Custom Proprietary License.
// Viewing is permitted. Copying, modifying, or distributing
// without explicit permission is prohibited.
// For permissions, contact [lauriojohnangelo@gmail.com].
```

[Lesson05>>](/Lesson05/Topic01.md)


