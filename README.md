# Practical 7 - Understanding Linux Process Address Space

## Aim

To write a C program that prints the addresses of code, global, static, heap, and stack variables, and to analyze the corresponding regions of a Linux process address space.

## Files

### memory_layout.c

This program displays the addresses of:

- Code/Text
- Global/Data
- Static
- BSS
- Heap
- Stack

### memory_demo.c

This program keeps a process running so that its virtual memory mappings can be examined using the Linux `/proc` filesystem.

## Compilation

```bash
gcc -Wall -Wextra -g memory_layout.c -o memory_layout
gcc -Wall -Wextra -g memory_demo.c -o memory_demo
