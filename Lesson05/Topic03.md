# Pre-defined Math Functions
C++ programming provides a math library that contains a set of pre-defined mathematical functions. These functions are included in the `<cmath>` header file and allow you to perform various mathematical operations, such as calculating square roots, raising numbers to a power, and evaluating trigonometric functions. This guide introduces the most commonly used math library functions in C++, along with their usage and examples.

## Math Library Functions
### sqrt
The `sqrt` function is used to calculate the square root of a number. It takes a single argument and returns the square root as a `double` value. Here's an example:
```cpp
#include <iostream>
#include <cmath>

int main() {
	double num = 16;
	double result = std::sqrt(num);

	std::cout << "Square root of " << num << " is " << result << std::endl;

	return 0;
}
```
The output will be: "Square root of 16.00 is 4.00".

### pow
The pow function is used to raise a number to a power. It takes two arguments: the base number and the exponent. It returns the result as a `double` value. Here's an example:
```cpp
#include <iostream>
#include <cmath>

int main() {
	double base = 2;
	double exponent = 3;
	double result = std::pow(base, exponent);

	std::cout << base << " raised to the power of " << exponent << " is " << result << std::endl;

	return 0;
}
```
The output will be: "2.00 raised to the power of 3.00 is 8.00".

### sin and cos
The `sin` and `cos` functions are used to calculate the sine and cosine of an angle, respectively. These functions take the angle in radians as an argument and return the corresponding sine or cosine value as a `double` value. Here's an example:
```cpp
#include <iostream>
#include <cmath>

int main() {
	double angle = 0.5;
	double sin_result = std::sin(angle);
	double cos_result = std::cos(angle);

	std::cout << "Sine of " << angle << " is " << sin_result << std::endl;
	std::cout << "Cosine of " << angle << " is " << cos_result << std::endl;
	return 0;
}
```
The output will be: "Sine of 0.50 is 0.48" "Cosine of 0.50 is 0.88".

```cpp
// This Topic is licensed under a Custom Proprietary License.
// Viewing is permitted. Copying, modifying, or distributing
// without explicit permission is prohibited.
// For permissions, contact [lauriojohnangelo@gmail.com].
```

[Lesson06>>](/Lesson06/Topic01.md)
