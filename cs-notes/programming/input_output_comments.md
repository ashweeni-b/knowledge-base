### Input Output and Comments

#### Comments

- Non-executable statments written in the code 
- Ignored by the compiler during execution
- Explains program purpose, logic, author, date and notes
- Used in documentation section and body of the code

#### Types of Comments

1. Single-line comment

    ```c
    // This is a single-line comment
    ```

2. Multi-line comment

    ```c
    /*
    This is a
    multi-line 
    comment
    */
    ```

#### Input and Output

1. C

    In C, standard I/O library `<stdio.h>` is used

    Input:
    - `scanf()` - Reads input from keyboard
    - `getchar()` - Reads single character
    - `fgets()` - Reads whole line including spaces

    Output:
    - `printf()` - Prints the output
    - `putchar()` - Prints one character
    - `puts()` - Prints a string and adds a newline automatically

    ```c
    #include <stdio.h>

    int main() {
        // Input integer
        int a;
        scanf("%d", &a);

        // Output integer
        printf("%d", a);

        // Input character
        char ch = getchar();

        // Input line
        char ch[50];
        fgets(ch);

        // Print character
        putchar('A');

        // Prints line
        puts("HELLO");

        return 0;
    }
    ```

1. C++

    In C++, standard input/output stream library `<iostream>` is used

    Input:
    - `cin` - Reads input
    - `cin.ignore` - Discards character from the input buffer
    - `cin.fail` - Checks whether input failed
    - `getline()` - Reads a full line including spaces

    Output:
    - `cout` - Print the output
    - `cerr` - Prints the error message
    - `clog` - Prints logging and debug messages

```cpp
#include <iostream>

int main() {
    // Input integer
    int a;
    std::cin >> a;

    // Output integer
    std::cout << a;
    
    // Ignore input buffer
    int b;
    std::cin.ignore();   // Removes 1 character
    std::cin >> b;

    // Checks failure of input
    int c;
    std::cin >> c;
    // If entered value is character
    if(std::cin.fail()) {
        std::cout << "Invalid input";
    }

    // Input full line
    string name;
    getline(std::cin, name);

    // Print error and log messages
    float x;
    std::cin >> x;
    std::clog << "Program started";
    // If entered value is character
    if(std::cin.fail()) {
        std::err << "Error";
    }

    return 0;
}
```

#### Escape Sequences

- Special sequence of characters used in strings to represent characters that are difficult to enter directly
- Common escape sequences characters are:

1. Newline - \n
1. Tab - \t
1. Backslash - \\\\
1. Single quote - \\'
1. Dobule quote - \\"
1. Question mark - \\?

---