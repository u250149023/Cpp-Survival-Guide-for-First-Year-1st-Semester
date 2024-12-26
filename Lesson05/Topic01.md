## Pre-defined Character Functions

C++ offers a variety of built-in functions for manipulating characters. These functions enable you to perform different operations on characters, such as determining if a character is alphabetic or numeric, converting characters to uppercase or lowercase, and more. Mastering these character functions can significantly improve your ability to manage and manipulate character data in C++ programming. This guide outlines common character manipulation functions in C++, including their usage and examples.

## Common Character Manipulation Functions
### isalpha
The `isalpha` function in C++ checks whether a given character is an alphabetic character (A-Z or a-z). It returns a non-zero value if the character is alphabetic, otherwise it returns zero. Here's an example:
```cpp
#include <iostream>
#include <cctype>

int main() {
	std::cout << std::boolalpha;
	std::cout << std::isalpha('c') << '\n'; // displays true
	std::cout << std::isalpha('4') << '\n'; // displays false
	return 0;
}
```
### isdigit
The `isdigit` function in C++ checks whether a given character is a digit (0-9). It returns a non-zero value if the character is a digit, otherwise it returns zero. Here's an example:
```cpp
#include <iostream>
#include <cctype>

int main() {
	std::cout << std::boolalpha;
	std::cout << std::isdigit('4') << '\n'; // displays true
	std::cout << std::isdigit('c') << '\n'; // displays false
	return 0;
}
```
### toupper and tolower
The `toupper` and `tolower` functions in C++ convert a character to uppercase and lowercase, respectively. They return the converted character. Here's an example:
```cpp
#include <iostream>
#include <cctype>

int main() {
	char ch = 'a';

	std::cout << "Original character: " << ch << '\n'; // Original character: a
	std::cout << "Uppercase: " << static_cast<char>(std::toupper(ch)) << '\n'; // Uppercase: A
	std::cout << "Lowercase: " << static_cast<char>(std::tolower(ch)) << '\n'; // Lowercase: a

	return 0;
}
```
## Usage and Examples of Character Functions
### isalnum
The `isalnum` function in C++ checks whether a given character is alphanumeric (A-Z, a-z, or 0-9). It returns a non-zero value if the character is alphanumeric, otherwise it returns zero. Here's an example:
```cpp
#include <iostream>
#include <cctype>

int main() {
	std::cout << std::boolalpha;
	std::cout << std::isalnum('9') << '\n'; // displays true
	std::cout << std::isalnum('c') << '\n'; // displays true
	std::cout << std::isalnum('#') << '\n'; // displays false
	return 0;
}
```
### iscntrl
The `iscntrl` function in C++ checks whether a given character is a control character. Control characters are non-printable characters used to control the behavior of devices such as printers and terminals.

The `iscntrl` function returns a non-zero value if the character is a control character, and zero otherwise. Here's an example:
```cpp
#include <iostream>
#include <cctype>

int main() {
	std::cout << std::boolalpha;
	std::cout << std::iscntrl('\n') << '\n'; // displays true
	std::cout << std::iscntrl('A') << '\n';  // displays false
	return 0;
}
```
### islower and isupper
The `islower` function in C++ is used to determine whether a given character is a lowercase letter (a-z). On the other hand, `isupper` function is used to determine whether a given character is an uppercase letter (A-Z).

The `islower` function returns a non-zero value if the character is in lowercase, and zero otherwise. On the other hand, `isupper` function returns a non-zero value if the character is in uppercase, and zero otherwise. Here's an example:
```cpp
#include <iostream>
#include <cctype>

int main() {
	std::cout << std::boolalpha;
	std::cout << std::islower('c') << '\n'; // displays true
	std::cout << std::isupper('c') << '\n'; // displays false
	return 0;
}
```
### isspace
The `isspace` function in C++ checks whether a given character is a white space character (space, tab, newline, etc.). It returns a non-zero value if the character is a white space character, otherwise it returns zero. Here's an example:
```cpp
#include <iostream>
#include <cctype>

int main() {
	std::cout << std::boolalpha;
	std::cout << std::isspace('\n') << '\n'; // displays true
	std::cout << std::isspace('A') << '\n';  // displays false
	return 0;
}
```
### isprint
The `isprint` function in C++ is used to determine whether a given character is a printable character. Printable characters are those that can be displayed on the screen or printed. Here's an example:
```cpp
#include <iostream>
#include <cctype>

int main() {
	std::cout << std::boolalpha;
	std::cout << std::isprint('\n') << '\n'; // displays false
	std::cout << std::isprint('A') << '\n';  // displays true
	return 0;
}
```
### ispunct
The `ispunct` function in C++ is used to determine whether a given character is a punctuation character. Punctuation characters are those that are not alphanumeric or whitespace characters. Here's an example:
```cpp
#include <iostream>
#include <cctype>

int main() {
	std::cout << std::boolalpha;
	std::cout << std::ispunct('.') << '\n'; // displays true
	std::cout << std::ispunct('A') << '\n'; // displays false
	return 0;
}
```
### isxdigit
The `isxdigit` function in C++ is used to determine whether a given character is a hexadecimal digit (0-9, A-F, or a-f). Here's an example:
```cpp
#include <iostream>
#include <cctype>

int main() {
	std::cout << std::boolalpha;
	std::cout << std::isxdigit('f') << '\n'; // displays true
	std::cout << std::isxdigit('g') << '\n'; // displays false
	return 0;
}
```

```cpp
// This code is licensed under a Custom Proprietary License.
// Viewing is permitted. Copying, modifying, or distributing
// without explicit permission is prohibited.
// For permissions, contact [@lauriojohnangelo@gmail.com].
```

