# C Programming - Piscine Modules and Projects

This repository contains my solutions and technical documentation for foundational **C programming** modules (`C00` through `C06`) and the `Rush00` project. Each module is designed to build a deep, foundational understanding of computer science concepts, memory mechanics, pointer manipulation, command-line arguments, and algorithm implementation in C.

## 📂 Module Structure & Implementations

### c00 - Fundamentals & Basic Outputs
- **`ex00 (ft_putchar.c)`**: A fundamental utility function that prints a single character to the standard output using the low-level Unix `write` system call.
- **`ex01 (ft_print_alphabet.c)`**: Iterates through the ASCII table from `'a'` to `'z'` to print the lowercase alphabet in sequential order.
- **`ex02 (ft_print_reverse_alphabet.c)`**: Prints the lowercase alphabet in reverse order from `'z'` down to `'a'` using decrement loops.
- **`ex03 (ft_print_numbers.c)`**: Outputs digits from `'0'` to `'9'` sequentially using character-based iteration.
- **`ex04 (ft_is_negative.c)`**: Evaluates an integer parameter and outputs `'N'` if negative or `'P'` if positive/zero using conditional branching.
- **`ex05 (ft_print_comb.c)`**: Generates and prints all unique ascending combinations of three different digits (0 to 9) separated by commas, demonstrating nested loop algorithms.


### c01 - Pointers & Memory Mechanics
- **`ex00 (ft_ft.c)`**: Takes a pointer to an integer and sets its underlying value to `42`, introducing fundamental pointer dereferencing.
- **`ex01 (ft_ultimate_ft.c)`**: Takes a pointer to a pointer (up to 9 levels deep) and updates the target integer to `42`, reinforcing multi-level pointer navigation.
- **`ex02 (ft_swap.c)`**: Swaps the values of two integers in memory using their respective memory addresses (`int *a`, `int *b`).
- **`ex03 (ft_div_mod.c)`**: Performs integer division and modulo operations simultaneously, storing results through pointer parameters.
- **`ex04 (ft_ultimate_div_mod.c)`**: Computes division and modulo in-place, updating the variables directly via pointers.
- **`ex05 (ft_putstr.c)`**: Iterates through a null-terminated string and prints each character via the `write` system call.
- **`ex06 (ft_strlen.c)`**: Reimplementation of standard `strlen`, calculating the total character count until the null terminator (`\0`).

### c02 - String Manipulation & ASCII Validation
- **`ex00 (ft_strcpy.c)`**: Copies a source string into a destination character buffer, including the trailing null terminator.
- **`ex01 (ft_strncpy.c)`**: Copies up to `n` bytes from source to destination, padding with null bytes if necessary.
- **`ex02 (ft_str_is_alpha.c)`**: Validates if a string consists exclusively of alphabetic characters (`a-z`, `A-Z`).
- **`ex03 (ft_str_is_numeric.c)`**: Validates if a string contains only numeric digits (`0-9`).
- **`ex04 (ft_str_is_lowercase.c)`**: Checks whether all characters in a string are lowercase alphabetic characters.
- **`ex05 (ft_str_is_uppercase.c)`**: Checks whether all characters in a string are uppercase alphabetic characters.
- **`ex06 (ft_str_is_printable.c)`**: Validates that all characters in a string fall within the printable ASCII range (`32` to `126`).
- **`ex07 (ft_strupcase.c)`**: Converts all lowercase letters in a string to uppercase in-place using ASCII arithmetic (`- 32`).
- **`ex08 (ft_strlowcase.c)`**: Converts all uppercase letters in a string to lowercase in-place using ASCII arithmetic (`+ 32`).


### c03 - Advanced String Comparison & Searching
- **`ex00 (ft_strcmp.c)`**: Lexicographically compares two strings character by character, returning their ASCII difference.
- **`ex01 (ft_strncmp.c)`**: Compares up to `n` bytes of two strings with safety bounds.
- **`ex02 (ft_strcat.c)`**: Appends a source string to the end of a destination buffer, ensuring correct null termination.
- **`ex03 (ft_strncat.c)`**: Appends at most `n` bytes from a source string to a destination buffer safely.
- **`ex04 (ft_strstr.c)`**: Locates the first occurrence of a substring within a main string using nested iteration.

### c04 - Basic Conversions & Output Formatting
- **`ex00 (ft_strlen.c)`**: Calculates string length utility.
- **`ex01 (ft_putstr.c)`**: Outputs character streams using low-level writes.
- **`ex02 (ft_putnbr.c)`**: Recursively prints integers, handling edge cases like negative signs and extreme limits (`INT_MIN`).
- **`ex03 (ft_atoi.c)`**: Parses an ASCII string into a signed integer, managing leading whitespaces, signs, and valid digit sequences.


### c05 - Recursion & Mathematical Algorithms
- **`ex00 (ft_iterative_factorial.c)`**: Calculates a number's factorial iteratively using loops.
- **`ex01 (ft_recursive_factorial.c)`**: Computes a number's factorial using recursive function calls.
- **`ex02 (ft_iterative_power.c)`**: Computes power calculations (`nb^power`) via iterative loops.
- **`ex03 (ft_recursive_power.c)`**: Computes power calculations using recursive function patterns.
- **`ex04 (ft_fibonacci.c)`**: Computes the $n$-th element in the Fibonacci sequence using multi-branch recursion.
- **`ex05 (ft_sqrt.c)`**: Finds the exact integer square root of a number using iterative verification.
- **`ex06 (ft_is_prime.c)`**: Checks whether a number is prime by optimizing divisibility checks up to $\sqrt{nb}$.
- **`ex07 (ft_find_next_prime.c)`**: Locates the smallest prime number greater than or equal to the given input using helper functions.

### c06 - Command Line Arguments
- **`ex00 (ft_print_program_name.c)`**: Extracts and prints the executable path (`argv[0]`) of the running program.
- **`ex01 (ft_print_params.c)`**: Iterates through and outputs all command-line arguments provided after the program name, each on a new line.
- **`ex02 (ft_rev_params.c)`**: Outputs command-line arguments in reverse order, starting from the last argument down to the first.
- **`ex03 (ft_sort_params.c)`**: Sorts command-line arguments alphabetically using custom string comparisons and in-place sorting before printing.

### Rush00 - Dynamic Rectangle Drawing
- **`ft_putchar.c`**: Low-level character output helper using `write(1, &c, 1)`.
- **`rush00.c`**: Implements boundary logic (`drawo` for corners `'o'` and horizontal edges `'-'`, `drawi` for vertical side walls `'|'` and interior whitespace `' '`) along with strict coordinate validation (`x > 0`, `y > 0`).
- **`main.c`**: Entry point executing grid generation tests (e.g., `rush(123, 42)`).

## 🛠️ Compilation and Usage

All files are written in standard C and compile with standard compilation flags:

```bash
gcc -Wall -Wextra -Werror *.c
```

*Maintained by EmreQraz.*
