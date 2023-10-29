# Code Vulnerabilities

This repository is designed to store vulnerable code that can be exploited.

The code is not very complex, it's just for learning purposes, if you wish to run any of them, **you will need to comment** the other codes that are not supposed to be considered in the execution.

Explanations about the vulnerabilities can be found below:

1. **Buffer Overflow**:
    - **What it is**: A buffer overflow occurs when a program writes more data to a buffer (a temporary memory area) than the allocated size, potentially corrupting adjacent memory and allowing attackers to execute malicious code.
    - **Protection**: Use secure string manipulation functions like `strncpy` instead of `strcpy` and always check buffer boundaries. Utilize code analysis tools to identify potential buffer overflow vulnerabilities.

2. **Format String**:
    - **What it is**: A format string vulnerability occurs when an attacker can manipulate the format string in a formatting function (e.g., `printf`) to read or write data from the program's memory.
    - **Protection**: Avoid using untrusted format strings and always validate user input. Use functions that don't allow arbitrary format string manipulation, like `snprintf` instead of `printf`.

3. **Integer Overflow**:
    - **What it is**: Integer overflow occurs when an arithmetic operation results in a value that cannot be represented in the data type used to store it. This can lead to unexpected results and security vulnerabilities.
    - **Protection**: Always check boundaries and the results of arithmetic operations and use appropriate data types to store values. Implement checks and limitations on calculations that could lead to overflows.

4. **Null Pointer Dereference**:
    - **What it is**: A null pointer dereference occurs when a program attempts to access or manipulate memory at a memory address pointed to by a null (or uninitialized) pointer.
    - **Protection**: Always initialize pointers and ensure they are not null before accessing the memory they point to. Use defensive programming practices to avoid null pointers and use exceptions or error returns to handle such situations.
