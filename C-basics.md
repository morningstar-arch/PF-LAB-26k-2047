# C-Basics.md

## 1. Data Types

| Data Type | Description |
|-----------|-------------|
| `int` | Stores whole numbers (positive, negative, or zero) without decimal points. Typically 4 bytes. |
| `float` | Stores single-precision floating-point (decimal) numbers. Typically 4 bytes, ~6-7 significant digits. |
| `double` | Stores double-precision floating-point numbers. Typically 8 bytes, more precise than `float`. |
| `char` | Stores a single character (letter, digit, or symbol). Typically 1 byte. |
| `bool` | Stores a boolean value: `true` (1) or `false` (0). Requires `<stdbool.h>` in C. |
| `void` | Represents "no type" — used for functions that return nothing, or generic pointers. |

## 2. Format Specifiers

| Specifier | Meaning |
|-----------|---------|
| `%d` | Signed decimal integer |
| `%u` | Unsigned decimal integer |
| `%o` | Unsigned octal integer |
| `%x` | Unsigned hexadecimal integer (lowercase letters) |
| `%X` | Unsigned hexadecimal integer (uppercase letters) |
| `%f` | Floating-point number (decimal notation) |
| `%e` | Floating-point number (scientific/exponential notation) |
| `%c` | Single character |
| `%s` | String (character array) |
| `%ld` | Long signed decimal integer |

## 3. Input/Output Functions

- **`scanf()`** — Reads formatted input from the keyboard based on a format string (e.g. `scanf("%d", &num);`). Commonly used for numbers and single characters.
- **`printf()`** — Writes formatted output to the screen based on a format string (e.g. `printf("Value: %d\n", num);`).
- **`getchar()`** — Reads a single character from standard input and returns it as an `int`.
- **`putchar()`** — Writes a single character to standard output.
- **`fgets()`** — Reads a line of text (including spaces) from input into a character array, safely limiting the number of characters read — safer than `gets()`.
- **`puts()`** — Writes a string to standard output and automatically appends a newline.

## 4. Escape Sequences

| Escape Sequence | Meaning | Example |
|------------------|---------|---------|
| `\n` | New line | `printf("Hello\nWorld");` |
| `\t` | Horizontal tab | `printf("Name:\tAli");` |
| `\\` | Backslash character | `printf("Path: C:\\Users");` |
| `\'` | Single quote character | `printf("It\'s C");` |
| `\"` | Double quote character | `printf("\"Hello\"");` |

## 5. Precision

Precision for floating-point output is specified by placing a `.` followed by a number
between the `%` and the conversion character in the format specifier, e.g. `%.2f` prints
2 digits after the decimal point, `%.4f` prints 4 digits, and `%.6f` prints 6 digits.
If no precision is specified, `printf()` defaults to 6 digits after the decimal point for
`%f`. Precision controls how many digits appear after the decimal, not the total width of
the number.

Example:
```c
printf("%.2f\n", 3.14159);  // Output: 3.14
printf("%.4f\n", 3.14159);  // Output: 3.1416
```
