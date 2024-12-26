# Assignment Operators
**Assignment operators** are utilized to assign values to variables in programming languages, including C++. They offer a concise and efficient method to update a variable’s value based on a computation or another variable's value. C++ features various assignment operators, including the basic assignment operator (`=`) and compound assignment operators like `+=`, `-=`, `*=`, `/=`, and `%=`. This guide will cover how to use different assignment operators in C++ and provide examples to demonstrate their functionality.

## Different Assignment Operators
**Basic Assignment Operator** (`=`): The basic assignment operator is used to set a value for a variable. It places the value on the right side into the variable on the left side. For example:
```cpp
#include <iostream>

int main() {
	int num1 = 10;
	int num2 = 5;

	num1 += num2;   // Equivalent to num1 = num1 + num2
	std::cout << "num1 += num2: " << num1 << std::endl;

	num1 -= num2;   // Equivalent to num1 = num1 - num2
	std::cout << "num1 -= num2: " << num1 << std::endl;

	num1 *= num2;   // Equivalent to num1 = num1 * num2
	std::cout << "num1 *= num2: " << num1 << std::endl;

	num1 /= num2;   // Equivalent to num1 = num1 / num2
	std::cout << "num1 /= num2: " << num1 << std::endl;

	num1 %= num2;   // Equivalent to num1 = num1 % num2
	std::cout << "num1 %= num2: " << num1 << std::endl;

	return 0;
}
```
In the provided code, various assignment operators are used to change the value of `num1` based on `num2`, and then the updated values are displayed.

```cpp
// This Topic is licensed under a Custom Proprietary License.
// Viewing is permitted. Copying, modifying, or distributing
// without explicit permission is prohibited.
// For permissions, contact [lauriojohnangelo@gmail.com].
```

[NextTopic>>](./Topic03.md)
