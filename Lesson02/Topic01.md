# Arithmetic Operators
**Arithmetic operators** are key components of programming languages, including C++, enabling mathematical operations on numerical values. In C++, basic arithmetic operators are similar to those in C and include addition (`+`), subtraction (`-`), multiplication (`*`), division (`/`), and modulus (`%`). Additionally, C++ supports increment (`++`), decrement (`--`), and other arithmetic operations. Correct usage of these operators, along with an understanding of operator precedence and associativity, is essential for crafting accurate and efficient mathematical expressions in your programs. This guide will discuss the use of basic arithmetic operators in C++ and provide an overview of operator precedence and associativity.

## Basic Arithmetic Operators
- **Addition** (`+`): Adds two values together.
- **Subtraction** (`-`): Subtracts one value from another.
- **Multiplication** (`*`): Multiplies two values.
- **Division** (`/)`: Divides one value by another.
- **Modulus** (`%`): Computes the remainder after division.
- **Increment** (`++`): Increases the value of a variable by 1.
- **Decrement** (`--`): Decreases the value of a variable by 1.
```cpp
#include <iostream>

int main() {
	int a = 10, b = 5;
	int sum = a + b;		  // Addition
	int difference = a - b;   // Subtraction
	int product = a * b;	  // Multiplication
	int quotient = a / b;	 // Division
	int remainder = a % b;	// Modulus
	int increment = ++a;	  // Increment
	int decrement = --b;	  // Decrement

	std::cout << "Sum: " << sum << std::endl;
	std::cout << "Difference: " << difference << std::endl;
	std::cout << "Product: " << product << std::endl;
	std::cout << "Quotient: " << quotient << std::endl;
	std::cout << "Remainder: " << remainder << std::endl;
	std::cout << "Increment: " << increment << std::endl;
	std::cout << "Decrement: " << decrement << std::endl;

	return 0;
}
```
## Operator Precedence and Associativity
Operator precedence determines the order in which operators are evaluated in an expression. Operators with higher precedence are evaluated first. When multiple operators have the same precedence, the associativity of the operators comes into play. Associativity determines the order in which operators of the same precedence are evaluated, either from left to right or right to left.

1. Unary operators (e.g., `++`, `--`)
2. Multiplication (`*`), Division (`/`), Modulus (`%`)
3. Addition (`+`), Subtraction (`-`)

To avoid confusion and ensure the correct evaluation of expressions, you can use parentheses to explicitly specify the desired order of operations.

[NextTopic>>](./Topic02.md)
