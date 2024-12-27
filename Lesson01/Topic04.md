# Input Operations
Input operations in C++ allow programs to receive data from users or other sources. The `iostream` library provides tools for handling input and output (I/O) operations. The most commonly used input stream in C++ is `cin`, which stands for "character input".

## Input for Integers
To read an integer from the user, use the `cin` object along with the extraction operator `>>`.

Example:
```cpp
#include <iostream>
using namespace std;

int main() {
    int age;
    cout << "Enter your age: ";
    cin >> age;  // Read an integer value from the user and store it in the variable 'age'
    cout << "You entered: " << age << endl;  // Output the entered value
    return 0;
}
```

## Input for Strings
To read a string from the user, you can use cin for single words and getline for full lines.

Example for a Single Word:
```cpp
#include <iostream>
using namespace std;

int main() {
    string name;
    cout << "Enter your name: ";
    cin >> name;  // Read a single word input from the user and store it in the variable 'name'
    cout << "Hello, " << name << "!" << endl;  // Output the entered value
    return 0;
}
```

Example for a Full Line:
When you need to read a full line of text, including spaces, use getline. The ignore function is used to clear the input buffer.

```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string fullName;
    cout << "Enter your full name: ";
    getline(cin, fullName);  // Read a full line input from the user and store it in the variable 'fullName'
    cout << "Hello, " << fullName << "!" << endl;  // Output the entered value
    return 0;
}
```

## Combining Inputs
When combining different types of inputs using getline, you need to handle each input separately and perform any necessary conversions.

Example:
```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string name, input;
    int age;

    cout << "Enter your full name: ";
    getline(cin, name);  // Read a full line input for the name

    cout << "Enter your age: ";
    getline(cin, input);  // Read the input as a string
    age = stoi(input);  // Convert the string to an integer

    cout << "Hello, " << name << "! You are " << age << " years old." << endl;  // Output the entered values
    return 0;
}
```
### Advantages of Using getline
- **Handles Spaces**: `getline` can read entire lines, making it ideal for inputs that include spaces.
- **Consistent Input Handling**: Using `getline` consistently can simplify input handling logic, especially when processing mixed input types.

### Considerations
- **Manual Conversion**: When using `getline` for non-string inputs, you'll need to manually convert the string input to the desired data type (e.g., using `stoi` for integers).
- **Error Handling**: It's important to add error handling to manage invalid inputs, such as non-numeric strings when expecting an integer.

```cpp
// This Topic is licensed under a Custom Proprietary License.
// Viewing is permitted. Copying, modifying, or distributing
// without explicit permission is prohibited.
// For permissions, contact [lauriojohnangelo@gmail.com].
```

[Lesson02>>](/Lesson02/Topic01.md)

