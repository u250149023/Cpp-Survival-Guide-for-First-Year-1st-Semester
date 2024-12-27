# String Handling 
String handling in C++ involves various operations that you can perform on strings, such as concatenation, comparison, searching, and modifying. The string class in the C++ Standard Library provides a wide range of functionalities to manipulate strings efficiently.

## Basic String Operations

### Creating and Initializing Strings:
- You can create and initialize strings using the string class.

```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string str1 = "Hello";
    string str2("World");
    string str3 = str1 + " " + str2;  // Concatenation
    cout << str3 << endl;  // Output: Hello World
    return 0;
}
```

### String Length:
- Use the length() or size() member functions to get the length of a string.

```cpp
string str = "Hello, World!";
cout << "Length: " << str.length() << endl;  // Output: 13
```

### Accessing Characters:
- Access individual characters in a string using the [] operator or the at() member function.

```cpp
string str = "Hello";
cout << str[0] << endl;  // Output: H
cout << str.at(1) << endl;  // Output: e
```

### Modifying Strings:
- You can modify strings by changing individual characters, appending, or assigning new values.

```cpp
string str = "Hello";
str[0] = 'J';
cout << str << endl;  // Output: Jello
str.append(" World");
cout << str << endl;  // Output: Jello World
```

## Advanced String Operations
### Substring:
- Extract a substring from a string using the substr() member function.

```cpp
string str = "Hello, World!";
string sub = str.substr(7, 5);  // Extracts "World"
cout << sub << endl;  // Output: World
```

### Find:
- Search for a substring or character within a string using the find() member function.

```cpp
string str = "Hello, World!";
size_t pos = str.find("World");
if (pos != string::npos) {
    cout << "Found at position: " << pos << endl;  // Output: Found at position: 7
}
```

### Replace:
- Replace a part of the string with another string using the replace() member function.

```cpp
string str = "Hello, World!";
str.replace(7, 5, "C++");
cout << str << endl;  // Output: Hello, C++!
```

### Erase:
- Remove a portion of the string using the erase() member function.

```cpp
string str = "Hello, World!";
str.erase(5, 7);
cout << str << endl;  // Output: Hello
```
---

Here’s a comprehensive example demonstrating various string operations:

```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string str = "C++ Programming";

    // Length of the string
    cout << "Length: " << str.length() << endl;

    // Accessing characters
    cout << "First character: " << str[0] << endl;
    cout << "Second character: " << str.at(1) << endl;

    // Modifying the string
    str[0] = 'c';
    str.append(" is fun!");
    cout << str << endl;

    // Substring
    string sub = str.substr(4, 11);
    cout << "Substring: " << sub << endl;

    // Find
    size_t pos = str.find("fun");
    if (pos != string::npos) {
        cout << "'fun' found at position: " << pos << endl;
    }

    // Replace
    str.replace(pos, 3, "awesome");
    cout << "After replace: " << str << endl;

    // Erase
    str.erase(4, 11);
    cout << "After erase: " << str << endl;

    return 0;
}
```

```cpp
// This Topic is licensed under a Custom Proprietary License.
// Viewing is permitted. Copying, modifying, or distributing
// without explicit permission is prohibited.
// For permissions, contact [lauriojohnangelo@gmail.com].
```

[Lesson04>>](/Lesson04/Topic01.md)

