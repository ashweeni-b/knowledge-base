### Instructions

- Set of rules or sequences
- Types:
    - Type Declaration Instructions
    - Arithmetic Instructions
    - Control Instructions

#### Type Declaration Instructions
    
Instructs compiler to reserve memory location

```c
int a, k;
float b;
char ch;
int j = 1;
k = j + 1;     // Valid
int c = 4; d = 5;
f = a + b       // Invalid
int l, m, n, o;
l = m = n = o = 9;
```

#### Arithmetic Instructions

- Performs mathematical operations
- _Format:_ operand1 operator operand2 = value
- Common operators are:

    | Operator | Name |
    | ---- | ----- |
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
1. No operator for exponentiation

#### Control Instructions

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