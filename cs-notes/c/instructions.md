### Instructions

Set of rules or sequences

#### Types of Instructions

1. Type Declaration Instructions
    
    Instructs compiler to reserve memory location

    ```c
    int a; int j1;
    float b;
    char ch;
    int j = 1;
    j1 = j + 1;     // Valid
    int a2 = 4; b1 = 5;
    f = a + b       // Invalid
    int l, m, n, o;
    l = m = n = o = 9;
    ```

1. Arithmetic Instructions

    - Performs mathematical operations
    - Format: operand1 operator operand2 = value
    - Common operators are:

    | Operator | Name |
    | - | - |
    | + | Addition |
    | - | Subtraction |
    | * | Multiplication |
    | / | Division |
    | % | Modulus / Modulo |

    ```c
    a = b + c
    ```

    __Note:__

    1. Operands can be int, float, etc.
    1. Modulo cannot be applied on float
    1. Sign for the modulo operation is the same as the numerator
        ```c
        -5 % 3 = -2
        ```
    1. No operator is assumed
        ```c
        int i = a * b;      // Valid
        int j = ab;         // Invalid
        ```
    1. No operator for exponentiation in C. It can be done using _math.h_ library's _pow()_ function

1. Control Instructions

    Determines the flow of control in a program

    __Types of Control Instructions__

    1. Sequence Control Instructions

        Default mode of execution where instructions are executed one after another

    1. Decision Control Instructions

        Allows program to make decisions and execute different code paths based on conditions

    1. Loop Control Instructions

        Allows program to repeat a block of code multiple times

    1. Case Control Instructions

        Allows program to execute one of several code blocks based on value of variable

---

#### Type Conversion

Implicit conversion of data type from one to another <br />

int op int = int <br />
float op int = float <br />
float op float = float <br />

```c
// float gets demoted to int
int d = 6.7;
printf("%d", d);

// Output: 6
```

```c
// int gets promoted to float
float e = 8;
printf("%f", e);

// Output: 8.0
```

#### Type Casting

Explicit conversion of data type from one to another

```c
float m = 32.23;
int n = (int) m;
printf("%d", n);

// Output: 32
```

---