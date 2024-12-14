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

