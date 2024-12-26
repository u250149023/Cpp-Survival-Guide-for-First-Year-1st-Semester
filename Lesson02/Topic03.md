# Bitwise Operator
**Bitwise operators** in C++ work on the binary representation of numbers to perform tasks like bit manipulation, testing, and shifting. Key operators include AND (`&`), OR (`|`), XOR (`^`), complement (`~`), left shift (`<<`), and right shift (`>>`).

## Bitwise Operators
1. AND Operator (`&`): The AND operator compares two bits and returns 1 if both bits are 1, otherwise returns 0. Here's an example:
```cpp
1	    1010
2	&   0110
3	---------
4	    0010
```
2. OR Operator (`|`): The OR operator compares two bits and returns 1 if at least one of the bits is 1, otherwise returns 0. Here's an example:
```cpp
1	    1010
2	|   0110
3	---------
4	    1110
```
4. XOR Operator (`^`): The XOR operator compares two bits and returns 1 if the bits are different (one 0 and the other 1), otherwise returns 0. Here's an example:
```cpp
1	    1010
2	^   0110
3	---------
4	    1100
```
6. Complement Operator (`~`): The complement operator flips the bits, turning 0 to 1 and 1 to 0. Here's an example:
```cpp
1	~  1010
2	---------
3	   0101
```
7. Left Shift Operator (`<<`): The left shift operator shifts the bits of a number to the left by a specified number of positions, effectively multiplying the number by a power of 2. Here's an example:
```cpp
1	    1010 << 2
2	---------
3	    101000
```
8. Right Shift Operator (`>>`): The right shift operator shifts the bits of a number to the right by a specified number of positions, effectively dividing the number by a power of 2. Here's an example:
```cpp
1	    1010 >> 1
2	---------
3	    0101
```
---

```cpp
1	#include <iostream>
2	
3	int main() {
4	    unsigned int num1 = 10;    // Binary: 0000 1010
5	    unsigned int num2 = 6;     // Binary: 0000 0110
6	
7	    unsigned int result;
8	
9	    result = num1 & num2;      // Bitwise AND: 0000 0010 (2 in decimal)
10	    std::cout << "AND Result: " << result << std::endl;
11	
12	    result = num1 | num2;      // Bitwise OR: 0000 1110 (14 in decimal)
13	    std::cout << "OR Result: " << result << std::endl;
14	
15	    result = num1 ^ num2;      // Bitwise XOR: 0000 1100 (12 in decimal)
16	    std::cout << "XOR Result: " << result << std::endl;
17	
18	    result = ~num1;            // Bitwise complement: 1111 0101 (245 in decimal)
19	    std::cout << "Complement Result: " << result << std::endl;
20	
21	    result = num1 << 2;        // Left shift by 2: 0010 1000 (40 in decimal)
22	    std::cout << "Left Shift Result: " << result << std::endl;
23	
24	    result = num2 >> 1;        // Right shift by 1: 0000 0011 (3 in decimal)
25	    std::cout << "Right Shift Result: " << result << std::endl;
26	
27	    return 0;
28	}
```

```cpp
// This Topic is licensed under a Custom Proprietary License.
// Viewing is permitted. Copying, modifying, or distributing
// without explicit permission is prohibited.
// For permissions, contact [lauriojohnangelo@gmail.com].
```

[Lesson03>>](/Lesson03/Topic01.md)



