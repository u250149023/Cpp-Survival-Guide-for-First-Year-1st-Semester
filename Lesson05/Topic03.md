# Pre-defined Math Functions
The C++ Standard Library provides a variety of predefined math functions that are included in the <cmath> header. These functions cover a wide range of mathematical operations such as power, exponential, logarithmic, trigonometric, and other common mathematical calculations. Here's an overview of some of the most commonly used math functions.

## Common Predefined Math Functions
`sqrt(x)`:
Computes the square root of x.
```cpp
#include <iostream>
#include <cmath>
using namespace std;

int main() {
    double x = 16.0;
    cout << "Square root of " << x << " is " << sqrt(x) << endl;  // Output: Square root of 16 is 4
    return 0;
}
```

`pow(base, exponent)`:
- Computes the power of base raised to the exponent.
```cpp
double base = 2.0, exponent = 3.0;
cout << base << " raised to the power of " << exponent << " is " << pow(base, exponent) << endl;  // Output: 2 raised to the power of 3 is 8
```

`exp(x)`:
- Computes the exponential function e raised to the power x.
```cpp
double x = 1.0;
cout << "exp(" << x << ") is " << exp(x) << endl;  // Output: exp(1) is 2.71828
```

`log(x)`:
- Computes the natural logarithm (base e) of x.
```cpp
double x = 2.71828;
cout << "log(" << x << ") is " << log(x) << endl;  // Output: log(2.71828) is 1
```

`log10(x)`:
- Computes the common logarithm (base 10) of x.
```cpp
double x = 1000.0;
cout << "log10(" << x << ") is " << log10(x) << endl;  // Output: log10(1000) is 3
```

`sin(x), cos(x), tan(x)`:
- Compute the sine, cosine, and tangent of x (in radians), respectively.
```cpp
double x = M_PI / 4;  // 45 degrees in radians
cout << "sin(" << x << ") is " << sin(x) << endl;  // Output: sin(0.785398) is 0.707107
cout << "cos(" << x << ") is " << cos(x) << endl;  // Output: cos(0.785398) is 0.707107
cout << "tan(" << x << ") is " << tan(x) << endl;  // Output: tan(0.785398) is 1
```

`ceil(x)`:
- Rounds x up to the nearest integer.
```cpp
double x = 4.2;
cout << "ceil(" << x << ") is " << ceil(x) << endl;  // Output: ceil(4.2) is 5
```

`floor(x)`:
- Rounds x down to the nearest integer.
```cpp
double x = 4.8;
cout << "floor(" << x << ") is " << floor(x) << endl;  // Output: floor(4.8) is 4
```

`fabs(x)`:
- Computes the absolute value of x.
```cpp
double x = -5.3;
cout << "fabs(" << x << ") is " << fabs(x) << endl;  // Output: fabs(-5.3) is 5.3
```

`fmod(x, y)`:
- Computes the remainder of the division of x by y.
```cpp
double x = 5.3, y = 2.0;
cout << "fmod(" << x << ", " << y << ") is " << fmod(x, y) << endl;  // Output: fmod(5.3, 2) is 1.3
```

Here's a comprehensive example demonstrating various math functions:
```cpp
#include <iostream>
#include <cmath>
using namespace std;

int main() {
    double x = 16.0, y = 2.71828, z = 4.2;

    // Square root
    cout << "sqrt(" << x << ") = " << sqrt(x) << endl;

    // Power
    cout << "pow(" << y << ", 2) = " << pow(y, 2) << endl;

    // Exponential
    cout << "exp(1) = " << exp(1) << endl;

    // Natural logarithm
    cout << "log(" << y << ") = " << log(y) << endl;

    // Common logarithm
    cout << "log10(1000) = " << log10(1000) << endl;

    // Trigonometric functions
    cout << "sin(pi/4) = " << sin(M_PI / 4) << endl;
    cout << "cos(pi/4) = " << cos(M_PI / 4) << endl;
    cout << "tan(pi/4) = " << tan(M_PI / 4) << endl;

    // Ceiling and floor
    cout << "ceil(" << z << ") = " << ceil(z) << endl;
    cout << "floor(" << z << ") = " << floor(z) << endl;

    // Absolute value
    double neg = -5.3;
    cout << "fabs(" << neg << ") = " << fabs(neg) << endl;

    // Modulus
    cout << "fmod(5.3, 2) = " << fmod(5.3, 2) << endl;

    return 0;
}
```

Conclusion
The <cmath> header in C++ provides a rich set of predefined math functions that enable you to perform a wide range of mathematical operations efficiently.

```cpp
// This Topic is licensed under a Custom Proprietary License.
// Viewing is permitted. Copying, modifying, or distributing
// without explicit permission is prohibited.
// For permissions, contact [lauriojohnangelo@gmail.com].
```

[Lesson06>>](/Lesson06/Topic01.md)
