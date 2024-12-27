# Pre-defined Character Functions
The C++ Standard Library provides several predefined character functions for handling and manipulating individual characters. These functions are available in the `<cctype>` header and are commonly used for tasks such as checking character types and converting character cases.

## Common Predefined Character Functions
isalnum:
- Checks if the character is alphanumeric (a letter or a digit).

```cpp
#include <iostream>
#include <cctype>
using namespace std;

int main() {
    char ch = 'A';
    if (isalnum(ch)) {
        cout << ch << " is alphanumeric." << endl;
    } else {
        cout << ch << " is not alphanumeric." << endl;
    }
    return 0;
}
```

isalpha:
- Checks if the character is a letter.

```cpp
char ch = 'A';
if (isalpha(ch)) {
    cout << ch << " is a letter." << endl;
}
```

isdigit:
- Checks if the character is a digit.

```cpp
char ch = '5';
if (isdigit(ch)) {
    cout << ch << " is a digit." << endl;
}
```
islower:
- Checks if the character is a lowercase letter.

```cpp
char ch = 'a';
if (islower(ch)) {
    cout << ch << " is a lowercase letter." << endl;
}
```

isupper:
- Checks if the character is an uppercase letter.

```cpp
char ch = 'A';
if (isupper(ch)) {
    cout << ch << " is an uppercase letter." << endl;
}
```

isspace:
- Checks if the character is a whitespace character (such as space, tab, or newline).

```cpp
char ch = ' ';
if (isspace(ch)) {
    cout << "This is a whitespace character." << endl;
}
```

tolower:
- Converts a character to lowercase.

```cpp
char ch = 'A';
char lower = tolower(ch);
cout << ch << " in lowercase is " << lower << endl;  // Output: A in lowercase is a
```

toupper:
- Converts a character to uppercase.

```cpp
char ch = 'a';
char upper = toupper(ch);
cout << ch << " in uppercase is " << upper << endl;  // Output: a in uppercase is A
```

Example Program
Here's an example program demonstrating the use of these predefined character functions:

```cpp
#include <iostream>
#include <cctype>
using namespace std;

int main() {
    char ch = 'a';

    // Check if the character is alphanumeric
    if (isalnum(ch)) {
        cout << ch << " is alphanumeric." << endl;
    }

    // Check if the character is a letter
    if (isalpha(ch)) {
        cout << ch << " is a letter." << endl;
    }

    // Check if the character is a digit
    if (isdigit(ch)) {
        cout << ch << " is a digit." << endl;
    } else {
        cout << ch << " is not a digit." << endl;
    }

    // Check if the character is a lowercase letter
    if (islower(ch)) {
        cout << ch << " is a lowercase letter." << endl;
    }

    // Check if the character is an uppercase letter
    char upper = toupper(ch);
    if (isupper(upper)) {
        cout << ch << " converted to uppercase is " << upper << endl;
    }

    // Check if the character is a whitespace character
    if (isspace(' ')) {
        cout << "This is a whitespace character." << endl;
    }

    return 0;
}
```

Conclusion
The `<cctype>` header in C++ provides a range of predefined character functions that make it easy to check character types and perform conversions. These functions are invaluable for text processing and validation tasks.

```cpp
// This Topic is licensed under a Custom Proprietary License.
// Viewing is permitted. Copying, modifying, or distributing
// without explicit permission is prohibited.
// For permissions, contact [lauriojohnangelo@gmail.com].
```

[NextTopic>>](./Topic02.md)
