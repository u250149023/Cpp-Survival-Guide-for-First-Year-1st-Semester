# Pre-defined String Functions
C++ offers a variety of standard string functions that enable you to perform different operations on strings. These functions make string manipulation, searching, and other common tasks easier. By understanding and using these string functions, you can significantly improve your ability to manage and manipulate string data in C++ programming. This guide provides an overview of standard string functions, including their usage and examples.

## Standard String Functions

### size
The `size` function is used to determine the length of a string. It returns the number of characters in the string. Here's an example:
```cpp
#include <iostream>
#include <string>

int main() {
	std::string str = "Hello, World!";
	int length = str.size();

	std::cout << "Length of the string: " << length << std::endl;

	return 0;
}
```
The output will be: "Length of the string: 13".

### assign
The `assign` function is used to copy one string to another. It copies the contents of the source string to the destination string. Here's an example:
```cpp
#include <iostream>
#include <string>

int main() {
	std::string source = "Hello, World!";
	std::string destination;

	destination.assign(source);

	std::cout << "Copied string: " << destination << std::endl;

	return 0;
}
```
The output will be: "Copied string: Hello, World!".

### append
The `append` function is used to concatenate (append) two strings. It appends the contents of the source string to the end of the destination string, modifying the destination string. Here's an example:
#include <iostream>
#include <string>
```cpp
int main() {
	std::string destination = "Hello, ";
	std::string source = "World!";

	destination.append(source);

	std::cout << "Concatenated string: " << destination << std::endl;

	return 0;
}
```
The output will be: "Concatenated string: Hello, World!".

### compare
The `compare` function is used to compare two strings. It returns an integer value that indicates the relationship between the two strings. If the strings are equal, it returns 0. If the first string is less than the second string, it returns a negative value. If the first string is greater than the second string, it returns a positive value. Here's an example:
```cpp
#include <iostream>
#include <string>

int main() {
	std::string str1 = "banana";
	std::string str2 = "banana";

	int result = str1.compare(str2); // result will be 0
	
	std::cout << result << std::endl;
	return 0;
}
```
The output will be: "0".

## String Manipulation and Searching Operations
### find
The `find` function is used to search for a substring in a string. It returns the index of the first occurrence of the substring in the `string`, or `std::string::npos` if the substring is not found. Here's an example:
```cpp
#include <iostream>
#include <string>

int main() {
	std::string str = "Hello, World!";
	std::string substring = "World";

	size_t index = str.find(substring);

	if (index != std::string::npos) {
		std::cout << "Substring '" << substring << "' found at index " << index << std::endl;
	} else {
		std::cout << "Substring not found" << std::endl;
	}

	return

 0;
}
```
The output will be: "Substring 'World' found at index 7".

```cpp
// This code is licensed under a Custom Proprietary License.
// Viewing is permitted. Copying, modifying, or distributing
// without explicit permission is prohibited.
// For permissions, contact [@lauriojohnangelo@gmail.com].
```
