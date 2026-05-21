### Basic Concepts in C

#### Variables

- Container which stores a value
- Entity whose values can be changed
- Examples:
    ```c
    a = 5;
    b  = 3.0;
    c = 'A';
    ```

#### Rules for naming variables

1. First character must be an alphabet or underscore (_)
1. No commas and blanks are allowed
1. No special symbol other than underscore allowed
1. Variable names are case-sensitive
1. Variable names should be meaningful

#### Types of Variables

1. Integer variables - Stores integer
1. Real variables - Stores floating-point numbers
1. Character variables - Stores characters

```c
int a = 5;      // Integer variable
int b = 3;      // Real variable
float c = 4.2;  // Real variable
char ch = 'A';  // Character variable
```

---

#### Constants

- Entity whose values cannot change

#### Types of Constants 

1. Integer constant - 3, 4, 5, 9
1. Real constant - 3.14, 7.0, 5.6
1. Character constant - 'a', 'A', '#', '%'

---

#### Keywords

- Reserved words whose meaning is already known to the compiler
- C language has 32 keywords

| Keywords | | | |
| - | - | - | - |
| auto | double | int | stuct |
| break | long | else | switch |
| case | return | enum | typedef |
| char | register | extern | union |
| const | short | float | unsigned |
| continue | signed | for | void |
| default | sizeof | goto | volatile |
| do | static | if | while |

----

#### Comments

- Way to add notes to the program or clarify things
- Comments are ignored and not executed by the compiler

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

---

#### Datatypes

| Datatype | Format Specifier | Memory (in bytes) |
| - | - | - |
| Integer | %d | 4 |
| Float | %f | 4 |
| Character | %c | 1 |

The memory taken by the datatypes is checked using the ```sizeof()``` operator in C

---

#### Input and Output

1. Input 
    ```c
    scanf(Format specifier, &variable);
    ```
    Here, format specifier specifies the datatype of the variable, _&_ specifies that the value gets copied at the address indicated by the variable

1. Output
    ```c
    printf("Format specifier", variable);
    ```

    _Note:_ %8.1f denotes the floating-point number, where 8 denotes the imaginary box and 1 represents the number of digits to be printed after the decimal point

---

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