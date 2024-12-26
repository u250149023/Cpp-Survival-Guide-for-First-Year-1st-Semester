# Typecasting 

In C++ programming, typecasting, also called *type conversion*, is the process of changing a value from one data type to another. This allows you to adjust how a value is interpreted, enabling operations and assignments across different data types. This guide covers typecasting in C++, explaining its definition, purpose, and the two types: implicit and explicit. It also discusses converting between different data types.

**Typecasting** is the temporary conversion of a value's data type to carry out a specific operation or assignment that requires a different data type. This process ensures that operands in expressions are compatible, enables data manipulation in a desired format, and helps prevent data loss or truncation.

## Implicit typecasting 
also known as automatic type conversion, happens when the compiler converts a value from one data type to another without explicit instructions from the programmer. This process follows predefined rules set by the language. Implicit typecasting typically occurs when a smaller data type is assigned to a larger data type or when operations involve different data types. Here is an example:
```cpp
1	int a = 10;
2	double b = a;  // Implicit typecasting from int to double
```
In this example, the integer value `a` is implicitly converted to a floating-point value `b` during assignment.

## Explicit Typecasting
sometimes called type conversion, involves the programmer specifying the desired data type directly. This process uses a typecast operator to tell the compiler about the intended conversion. The format for explicit typecasting is `static_cast<desired_type>(value)`. Here is an example:
```cpp
1	double c = 3.14;
2	int d = static_cast<int>(c);  // Explicit typecasting from double to int
```
In this example, the floating-point value `c` is explicitly converted to an integer value `d` using the `static_cast<int>` operator.

## Casting Between Different Data Types
**Converting between data types** in C++ enables you to change how a value is interpreted and represented. It's important to recognize the constraints and potential hazards of casting, as it can lead to data loss, truncation, or unpredictable behavior. Here are some examples of casting between different data types:
```cpp
1	int x = 65;
2	char y = static_cast<char>(x);  // Explicitly casting int to char
3	
4	double a = 3.14;
5	int b = static_cast<int>(a);  // Explicitly casting double to int
6	
7	int p = 100;
8	float q = static_cast<float>(p);  // Explicitly casting int to float
```
In these examples, the values are explicitly casted to the desired data types using the `static_cast` operator. Now, let's further explore explicit typecasting between `char` and `int` in handling ASCII values:
```cpp
#include <iostream>

int main() {
	char ch = 'A'; // A character 'A'
	int asciiValue = static_cast<int>(ch); // Explicitly casting char to int to get ASCII value

	std::cout << "Character: " << ch << std::endl;
	std::cout << "ASCII Value: " << asciiValue << std::endl;

	// Now, let's do the reverse: casting from int (ASCII value) back to char
	int anotherAsciiValue = 98;
	char anotherChar = static_cast<char>(anotherAsciiValue); // Explicitly casting int to char

	std::cout << "ASCII Value: " << anotherAsciiValue << std::endl;
	std::cout << "Character: " << anotherChar << std::endl;

	return 0;
}
```
In this example, we start with the character `'A'` and explicitly cast it to an int, resulting in the ASCII value `65`. Then, we perform the reverse operation by explicitly casting an integer `98` back to a `char`, which corresponds to the character `'b'`.

```cpp
// This Topic is licensed under a Custom Proprietary License.
// Viewing is permitted. Copying, modifying, or distributing
// without explicit permission is prohibited.
// For permissions, contact [lauriojohnangelo@gmail.com].
```

[Lesson05>>](/Lesson05/Topic01.md)


