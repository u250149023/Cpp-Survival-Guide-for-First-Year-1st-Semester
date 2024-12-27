# Basic Escape Sequences
Escape sequences are special characters used in strings to represent certain actions or characters that cannot be typed directly. These sequences start with a backslash (`\`) followed by a specific character. Here's a rundown of some basic escape sequences in C++:

`\n` - Newline:
Moves the cursor to the next line.
```cpp
cout << "Hello\nWorld";  // Outputs: Hello
                         //          World
 ```
                        
`\t` - Horizontal Tab:
Inserts a tab space.
```cpp
cout << "Hello\tWorld";  // Outputs: Hello   World
```

`\b` - Backspace:
Moves the cursor one position back, effectively deleting the character before it.
```cpp
cout << "Hello\bWorld";  // Outputs: HellWorld
```

`\\` - Backslash:
Inserts a backslash character (\).
```cpp
cout << "This is a backslash: \\";  // Outputs: This is a backslash: \
```

`\"` - Double Quote:
Inserts a double-quote character (").
```cpp
cout << "She said, \"Hello World!\"";  // Outputs: She said, "Hello World!"
```

`\r` - Carriage Return:
Moves the cursor to the beginning of the current line.
```cpp
cout << "Hello\rWorld";  // Outputs: World
```

`\f` - Form Feed:
Advances the cursor to the next page (used in printers).
```cpp
cout << "Hello\fWorld";  // Effects vary, often not visible in modern consoles
```

`\a` - Alert (Bell):
Produces an alert sound or beep.
```cpp
cout << "\a";  // Outputs an alert sound (if the system supports it)
```

Here’s an example that uses multiple escape sequences:
```cpp
#include <iostream>
using namespace std;

int main() {
    cout << "Line 1\nLine 2" << endl;           // Newline
    cout << "Column1\tColumn2" << endl;         // Horizontal Tab
    cout << "Delete\b this" << endl;            // Backspace
    cout << "Backslash: \\" << endl;            // Backslash
    cout << "Quote: \"" << endl;                // Double Quote
    cout << "Carriage\rReturn" << endl;         // Carriage Return
    cout << "Form Feed\fTest" << endl;          // Form Feed
    cout << "Alert\a" << endl;                  // Alert (Bell)

    return 0;
}
```

```cpp
// This Topic is licensed under a Custom Proprietary License.
// Viewing is permitted. Copying, modifying, or distributing
// without explicit permission is prohibited.
// For permissions, contact [lauriojohnangelo@gmail.com].
```

[NextTopic>>](./Topic04.md)
