# ft_printf

# ft_printf Project Guide

## Introduction

The `ft_printf` project is a comprehensive exercise in implementing a simplified version of the standard C library's `printf` function in C. This guide provides an overview of the project, its purpose, how to get started, and advanced topics for customization and improvement.

## Project Overview

In the `ft_printf` project, you are tasked with creating a function, `ft_printf`, that mimics the behavior of the `printf` function in C. This function allows you to format and print various types of data, such as strings, numbers, and other objects, to the standard output or a file stream.

## Getting Started

### Prerequisites

To work with the `ft_printf` project, you need the following prerequisites:

- A Unix-like operating system (Linux, macOS, or similar).
- A C compiler (e.g., GCC).

### Installation

1. Clone the GitHub repository to your local machine:

   ```bash
   git@github.com:99shandhokhan88/ft_printf.git
   ```

2. Navigate to the project directory:

   ```bash
   cd ft_printf
   ```

3. Compile the project:

   ```bash
   make
   ```

## Usage

### Function Description

The `ft_printf` function mimics the behavior of the standard `printf` function. The function signature is as follows:

```c
int ft_printf(const char *format, ...);
```

- `format`: A string that specifies the format of the output, including placeholders for values to be inserted.
- Additional arguments: Values to be inserted into the format string based on format specifiers.

The function returns the number of characters printed (excluding the null-terminating character).

### Example Usage

Here's an example of how to use the `ft_printf` function:

```c
#include "ft_printf.h"

int main(void)
{
    char *name = "Venelin";
    int age = 420;

    ft_printf("Hello, my name is %s, and I am %d years old.\n", name, age);

    return 0;
}
```

## Customization

You can customize the `ft_printf` project by adding support for additional format specifiers or modifying the behavior of existing ones. Explore options for formatting and displaying data to meet your specific requirements.

## Advanced Topics

### Format Specifiers

Understand the use of format specifiers in the `ft_printf` function. Customize and extend the list of supported format specifiers to handle various data types and formatting options.

### Memory Management

Efficient memory management is important when dealing with strings and dynamic memory allocation. Explore techniques for managing memory associated with formatted output, such as allocating and freeing memory appropriately.

## Contributing

Contributions to the `ft_printf` project are welcome. Feel free to open issues, suggest improvements, or submit pull requests.

## License

This project is licensed under the MIT License.

This guide provides a comprehensive overview of the `ft_printf` project, from installation to customization and advanced topics. Adapt it for your repository's README file and keep it updated with any project changes or improvements.




# ft_printf Bonuses

While the basic requirements involve supporting the standard format specifiers like `%s`, `%d`, and `%c`, the bonus part of the project allows you to extend the functionality. Here's a guide and explanation for some common `ft_printf` bonuses:

### 1. **Handling Additional Format Specifiers:**

   - **Bonus: %b (Binary Format):** Extend `ft_printf` to support the `%b` format specifier, which allows you to print integer values in binary format.

   - **Bonus: %o (Octal Format):** Add support for the `%o` format specifier, which prints integers in octal (base 8) format.

   - **Bonus: %x and %X (Hexadecimal Format):** Implement `%x` and `%X` to print integers in lowercase and uppercase hexadecimal format, respectively.

### 2. **Handling Additional Flags:**

   - **Bonus: '#' Flag:** Implement the `#` flag for various format specifiers to control the output format. For example, with `%#x`, the output could include a "0x" prefix for hexadecimal numbers.

   - **Bonus: ' ' (Space) Flag:** Add support for the space flag, which inserts a space character before positive numbers to align them with negative numbers.

### 3. **Handling Length Modifiers:**

   - **Bonus: hh, h, l, and ll Length Modifiers:** Extend `ft_printf` to support these length modifiers for integer specifiers. For example, `%hd` and `%lld` for short and long long integers.

### 4. **Handling Floating-Point Numbers:**

   - **Bonus: %f Format Specifier:** Implement support for floating-point numbers using the `%f` format specifier. You may need to handle precision, rounding, and exponent notation.

### 5. **Handling Additional Specifiers:**

   - **Bonus: %p (Pointer Format):** Add support for the `%p` format specifier to print memory addresses.

   - **Bonus: %r (Non-printable Characters):** Implement a custom format specifier `%r` that can print non-printable characters as escape sequences (e.g., newline as `\n`).

### 6. **Color and Styling:**

   - **Bonus: Color Codes:** Allow the use of color codes in the format string, which can be used to change text color, background color, or apply other styling effects to the printed text.

### 7. **Dynamic Width and Precision:**

   - **Bonus: * (Dynamic Width and Precision):** Extend `ft_printf` to support dynamic width and precision using the `*` specifier. For example, `%*.*f` could allow you to specify width and precision as arguments.

### 8. **Additional Error Handling:**

   - **Bonus: Improved Error Handling:** Enhance error handling by returning meaningful error codes or messages when unexpected format strings or arguments are encountered.

### 9. **Performance Optimization:**

   - **Bonus: Performance Improvements:** Optimize your `ft_printf` implementation for speed and memory usage. Consider ways to reduce the number of function calls or memory allocations.

### 10. **Documentation and Testing:**

   - **Bonus: Comprehensive Documentation:** Document your `ft_printf` implementation thoroughly, including how to use the new format specifiers and flags.

   - **Bonus: Rigorous Testing:** Create a suite of test cases to ensure that your extended `ft_printf` handles all the new features correctly and doesn't introduce regressions in existing functionality.

Remember that the exact requirements for the bonus part of the `ft_printf` project may vary depending on your course or assignment guidelines. Always check the specific requirements provided to you. Additionally, make sure to maintain good coding practices, readability, and efficiency throughout your project.
