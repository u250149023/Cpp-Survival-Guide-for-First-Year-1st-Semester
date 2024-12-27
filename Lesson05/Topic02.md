# Pre-defined String Functions
The C++ Standard Library provides a variety of predefined string functions that facilitate string manipulation and processing. These functions are available through the string class and are highly useful for common string operations such as concatenation, comparison, searching, and modification.

## Common Predefined String Functions
`length()` / `size()`:
- Returns the length (number of characters) of the string.
```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string str = "Hello, World!";
    cout << "Length: " << str.length() << endl;  // Output: 13
    return 0;
}
```

`substr(start, length)`:
- Returns a substring starting from the specified position with the specified length.
```cpp
string str = "Hello, World!";
string sub = str.substr(7, 5);  // Extracts "World"
cout << "Substring: " << sub << endl;  // Output: World
```

`find(str)`:
- Searches for the specified substring and returns the position of the first occurrence.
```cpp
string str = "Hello, World!";
size_t pos = str.find("World");
if (pos != string::npos) {
    cout << "'World' found at position: " << pos << endl;  // Output: 'World' found at position: 7
}
```

`replace(start, length, str)`:
- Replaces a portion of the string starting from the specified position with the specified length with another string.
```cpp
string str = "Hello, World!";
str.replace(7, 5, "C++");
cout << "After replace: " << str << endl;  // Output: Hello, C++!
```

`erase(start, length)`:
- Removes a portion of the string starting from the specified position with the specified length.
```cpp
string str = "Hello, World!";
str.erase(5, 7);
cout << "After erase: " << str << endl;  // Output: Hello
```

`append(str)`:
- Appends the specified string to the end of the current string.
```cpp
string str = "Hello";
str.append(", World!");
cout << "After append: " << str << endl;  // Output: Hello, World!
```

`compare(str)`:
- Compares the current string with the specified string lexicographically. Returns 0 if equal, a negative value if less, and a positive value if greater.

```cpp
string str1 = "Hello";
string str2 = "World";
int result = str1.compare(str2);
if (result == 0) {
    cout << "Strings are equal" << endl;
} else if (result < 0) {
    cout << "str1 is less than str2" << endl;
} else {
    cout << "str1 is greater than str2" << endl;
}
```

`c_str()`:
- Returns a pointer to a null-terminated C-style string.
```cpp
string str = "Hello";
const char* cstr = str.c_str();
cout << "C-style string: " << cstr << endl;  // Output: Hello
```

Here's a comprehensive example demonstrating various string functions:
```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string str = "C++ Programming";

    // Length of the string
    cout << "Length: " << str.length() << endl;

    // Substring
    string sub = str.substr(4, 11);
    cout << "Substring: " << sub << endl;

    // Find
    size_t pos = str.find("Programming");
    if (pos != string::npos) {
        cout << "'Programming' found at position: " << pos << endl;
    }

    // Replace
    str.replace(pos, 11, "Coding");
    cout << "After replace: " << str << endl;

    // Erase
    str.erase(4, 6);
    cout << "After erase: " << str << endl;

    // Append
    str.append(" is fun!");
    cout << "After append: " << str << endl;

    // Compare
    string str2 = "C++ Coding is fun!";
    int result = str.compare(str2);
    if (result == 0) {
        cout << "Strings are equal" << endl;
    } else if (result < 0) {
        cout << "str is less than str2" << endl;
    } else {
        cout << "str is greater than str2" << endl;
    }

    // C-style string
    const char* cstr = str.c_str();
    cout << "C-style string: " << cstr << endl;

    return 0;
}
```

Conclusion
The string class in C++ provides a rich set of predefined functions to handle and manipulate strings efficiently. These functions enable you to perform a wide range of operations, from simple concatenation to complex searching and modification.

```cpp
// This Topic is licensed under a Custom Proprietary License.
// Viewing is permitted. Copying, modifying, or distributing
// without explicit permission is prohibited.
// For permissions, contact [lauriojohnangelo@gmail.com].
```

[NextTopic>>](./Topic03.md)
