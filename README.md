# ft_printf - Custom Printf Implementation

A recreation of the printf function from the C standard library as part of the 42 curriculum.

## 📋 Overview

This project implements a custom version of the printf function, supporting various format specifiers and conversions.

### 🔍 Supported Format Specifiers

- `%c` - Single character
- `%s` - String
- `%p` - Pointer address
- `%d` - Decimal (signed) integer
- `%i` - Integer
- `%u` - Unsigned decimal integer
- `%x` - Hexadecimal (lowercase)
- `%X` - Hexadecimal (uppercase)
- `%%` - Percentage sign

## 📁 Files Structure

- `ft_printf.c` - Main printf implementation
- `ft_printf.h` - Header file with prototypes
- `print_characters.c` - Character and string handling
- `print_hex.c` - Hexadecimal conversion handlers
- `print_numbers.c` - Integer handling
- `print_unsigned_int.c` - Unsigned integer handling

## 🛠️ Usage

1. Compile the library:
```bash
make
```

2. Include in your project:
```c
#include "ft_printf.h"
```

3. Example usage:
```c
int main(void)
{
    ft_printf("Hello %s! Number: %d\n", "World", 42);
    ft_printf("Hex: %x, Pointer: %p\n", 255, &var);
    return (0);
}
```

## ⚙️ Build Instructions

- `make` - Compile the library
- `make clean` - Remove object files
- `make fclean` - Remove object files and library
- `make re` - Recompile everything

## 🔄 Return Value

Returns the number of characters printed (excluding the null byte used to end output to strings).

## 📝 Notes

- Handles basic format specifiers without flags/precision/width
- Thread-safe implementation
- No memory leaks
- Follows 42 Norm coding standards

## 📜 License

This project is part of the 42 curriculum and is provided as-is.
