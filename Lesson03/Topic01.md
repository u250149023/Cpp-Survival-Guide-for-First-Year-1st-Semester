# String Handling 
In C++, strings are character sequences commonly used for handling and manipulating text data. String operations include concatenation, comparison, copying, and more. This guide offers an overview of string handling in C++ programming, delves into common string operations, and presents string functions available in the standard library.

## Definition and Properties of Strings
In C++, strings are handled by the `std::string` class from the C++ Standard Library. Here are some key characteristics of these strings:

- **Strings are mutable**: Unlike in C, where strings cannot be altered without creating a new string, C++ strings can be directly modified.
- **Strings are not null-terminated**: The `std::string` class in C++ manages the length of the string internally, so there's no need for a null character.

## String Operations
### String Input
String input is the process of obtaining a sequence of characters (a string) from a user or an input source. In C++, you can use the `std::cin` object along with the `>>` extraction operator to read strings from the standard input. Here's an example:
```cpp
1.  #include <iostream>
2.  #include <string>
3.
4.  int main() {
5.      std::string name;
6.
7.      std::cout << "Enter your name: ";
8.      std::cin >> name;
9.
10.     std::cout << "Hello, " << name << "!\n";
11.
12.     return 0;
13. }
```
---
### String Concatenation
String concatenation is the process of combining two or more strings into a single string. In C++, you can concatenate strings using the `+` operator or the `append` member function of the `std::string` class. Here's an example:
```cpp
1.  #include <iostream>
2.  #include <string>
3.
4.  int main() {
5.      std::string str1 = "Hello";
6.      std::string str2 = "World";
7.
8.      std::string result = str1 + str2;
9.
10.     std::cout << "Concatenated string: " << result << "\n";
11.
12.     return 0;
13. }
```
The output will be: "HelloWorld".

---
### String Comparison
String comparison is used to determine the order or equality of two strings. In C++, you can compare strings using the comparison operators (`<`, `>`, `<=`, `>=`, `==`, `!=`) or the `compare` member function of the `std::string` class. Here's an example:
```cpp
1.  #include <iostream>
2.  #include <string>
3.
4.  int main() {
5.      std::string str1 = "banana";
6.      std::string str2 = "banana";
7.
8.      int result = str1.compare(str2); // result will be 0
9.
10.     std::cout << result << "\n";
11.
12.     return 0;
13. }
```
The output will be: "0" (indicating that the strings are equal).

---
### String Copying
String copying involves copying the contents of one string to another. In C++, you can simply assign one string to another using the assignment operator (`=`). Here's an example:
```cpp
1.  #include <iostream>
2.  #include <string>
3.
4.  int main() {
5.      std::string str1 = "Hello";
6.      std::string str2;
7.
8.      str2 = str1;
9.
10.     std::cout << "Copied string: " << str2 << "\n";
11.
12.     return 0;
13. }
```
The output will be: "Hello".

```cpp
// This Topic is licensed under a Custom Proprietary License.
// Viewing is permitted. Copying, modifying, or distributing
// without explicit permission is prohibited.
// For permissions, contact [lauriojohnangelo@gmail.com].
```

[Lesson04>>](/Lesson04/Topic01.md)

