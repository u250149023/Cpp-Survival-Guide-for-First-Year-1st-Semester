# Basic Escape Sequences
**Escape sequences** are unique character combinations that let you represent characters which are hard to type or have special meanings within a string. In C++ programming, these sequences help to include characters that can’t be directly typed into a string. This guide will discuss common escape sequences in C++, how to use them, and provide examples to showcase their functionality.

## Common Escape Sequences
- `\n`: Newline - Moves the cursor to the beginning of the next line.
- `\t`: Tab - Inserts a horizontal tab.
- `\"`: Double quote - Inserts a double quote character.
- `\'`: Single quote - Inserts a single quote character.
- `\\`: Backslash - Inserts a backslash character.
- `\b`: Backspace - Moves the cursor back one position.
- `\r`: Carriage return - Moves the cursor to the beginning of the current line.
- `\f`: Form feed - Moves the cursor to the next logical page.
```cpp
1.  #include <iostream>
2.  
3.  int main() {
4.      std::cout << "This is a new line.\n";
5.      std::cout << "Hello\tworld!\n";
6.      std::cout << "She said, \"Hello!\"\n";
7.      std::cout << "He said, 'I'm happy.'\n";
8.      std::cout << "This is a backslash: \\ \n";
9.      std::cout << "Hello\bWorld\n";
10.     std::cout << "Carriage return:\rOverwritten text\n";
11.     std::cout << "Form feed:\fHello\fWorld\n";
12. 
13.     return 0;
14. }
```
In the above code, each `std::cout` statement demonstrates the usage of a different escape sequence. The output will display the corresponding special characters and their effects.

```cpp
// This code is licensed under a Custom Proprietary License.
// Viewing is permitted. Copying, modifying, or distributing
// without explicit permission is prohibited.
// For permissions, contact [@lauriojohnangelo@gmail.com].
```

[NextTopic>>](./Topic04.md)
