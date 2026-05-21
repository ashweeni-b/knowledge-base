### Operators

#### Types of Operators

1. Arithmetic Operators

    | Operator | Name |
    | - | - |
    | + | Addition |
    | - | Subtraction |
    | * | Multiplication |
    | / | Division |
    | % | Modulus or Modulo |

1. Assignment Operators

    These are the compound assignment operators

    | Operator | Use | Shorthand |
    | - | - | - |
    | += | a = a + b | a += b |
    | -= | a = a - b | a -= b |
    | *= | a = a * b | a *= b |
    | /= | a = a / b | a /= b |
    | %= | a = a % b | a %= b |
    
    __Increment and Decrement Operator__

    | Operator | Name | Description |
    | - | - | - |
    | ++ | Increment | a = a + 1; Increment the value by 1 |
    | ++a | Pre-increment | Increments the value by 1 and then store it in a |
    | a++ | Post-increment | Stores the value in a and then increment it by 1 |
    | -- | Decrement | a = a - 1; Decrement the value by 1 |
    | --a | Pre-decrement | Decrements the value by 1 and then stores it in a |
    | a-- | Post-decrement | Stores the value in a and then decrement it by 1 |

    ```c
    int a = 4;
    printf("%d", a);        // 4
    printf("%d", ++a);      // 5
    printf("%d", a++);      // 5
    printf("%d", a);        // 6
    printf("%d", --a);      // 5
    printf("%d", a--);      // 5
    ```

1. Relational Operators

    | Operator | Name |
    | - | - |
    | > | Greater than |
    | >= | Greater than equal to |
    | < | Less than |
    | <= | Less than equal to |
    | == | Equal to |
    | != | Not equal to |

1. Logical Operators

    | Operators | Name |
    | - | - |
    | && | Logical AND |
    | \|\| | Logical OR |
    | ! | Logical NOT |

    These operators follows the following truth tables

    | A | B | A && B |
    | - | - | - |
    | 0 | 0 | 0 |
    | 0 | 1 | 0 |
    | 1 | 0 | 0 |
    | 1 | 1 | 1 |

    | A | B | A \|\| B |
    | - | - | - |
    | 0 | 0 | 0 |
    | 0 | 1 | 1 |
    | 1 | 0 | 1 |
    | 1 | 1 | 1 |

    | A | !A |
    | - | - |
    | 0 | 1 |
    | 1 | 0 |

1. Bitwise Operators

    | Operators | Name |
    | - | - |
    | & | Bitwise AND |
    | \| | Bitwise OR |
    | ^ | Exclusive XOR |

    These operators follows the following truth tables

    | A | B | A & B |
    | - | - | - |
    | 0 | 0 | 0 |
    | 0 | 1 | 0 |
    | 1 | 0 | 0 |
    | 1 | 1 | 1 |

    | A | B | A \| B |
    | - | - | - |
    | 0 | 0 | 0 |
    | 0 | 1 | 1 |
    | 1 | 0 | 1 |
    | 1 | 1 | 1 |

    | A | B | A ^ B |
    | - | - | - |
    | 0 | 0 | 0 |
    | 0 | 1 | 1 |
    | 1 | 0 | 1 |
    | 1 | 1 | 0 |

1. Ternary Operator

    ```c
    condition ? Statement 1 : Statement 2
    ```

    - It is a shortform of using if-else statement with single condition check.
    - If the condition is _True_, Statement 1 will be executed and if it is _False_, Statement 2 will be executed
    - Nested ternary operators can also be used for using multiple conditions, but that is not advisable.

#### Operator Precedence

| Priority | Operators |
| - | - |
| 1 | ! |
| 2 | * / % |
| 3 | + - |
| 4 | < <= > >= |
| 5 | == != |
| 6 | && | 
| 7 | \|\| |
| 8 | = |

Logical NOT, then Arithmetic, then Relational, then Logical and then Assignment operator (=)

#### Operator Associativity

Operator with same precedence follows left to right associativity and assignment operator (=) follows right to left associativity

$$
\begin{aligned}
& 3 * 6 / 2 * 9 + 7 * 3 \\
& = 18 / 2 * 9 + 7 * 3 \\
& = 9 * 9 + 7 * 3 \\
& = 81 + 7 * 3 \\
& = 81 + 21 \\
& = 102 
\end{aligned}
$$

---