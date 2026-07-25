### Operators

#### Unary Operators

| Operator | Name | Purpose |
| ----- | ----- | ----- |
| ++ | Increment | Increments the current value |
| ++a | Pre-increment | Increments and then uses the value |
| a++ | Post-increment | Uses and then increments the value |
| \-\- | Decrement | Decrements the current value |
| \-\-a | Pre-decrement | Decrements and then uses the value |
| a\-\- | Post-decrement | Uses and then decrements the value |

Here a is the operand and ++ or \-\- is the unary operator

```cpp
int a = 4;
std::cout << a;       // 4
std::cout << ++a;     // 5
std::cout << a++;     // 5
std::cout << a;       // 6
std::cout << --a;     // 5
std::cout << a--;     // 5
```

#### Binary Operators

- Has two operands and one operators
- Types:
    - Arithmetic operator
    - Assignment operator
    - Relational operator
    - Logical operator
    - Bitwise operator
    - Ternary operator

#### Arithmetic Operators

| Operator | Name |
| ----- | ----- |
| + | Addition |
| - | Subtraction |
| * | Multiplication |
| / | Division |
| % | Modulo |

% works only on integers and not on floating-point numbers

#### Assignment Operators

These are the compound assignment operators

| Operator | Name | Purpose |
| ----- | ----- | ----- |
| = | Equal to | a = 5 | 
| += | Plus equal to | a = a + b &rarr; a += b |
| -= | Minus equal to | a = a - b &rarr; a -= b |
| *= | Multiply equal to | a = a * b &rarr; a *= b |
| /= | Division equal to | a = a / b &rarr; a /= b |
| %= | Modulo equal to | a = a % b &rarr; a %= b |

#### Relational Operators

- Used for comparison
- Output 1 &rarr; True <br />
    Output 0 &rarr; False

| Operator | Name |
| ----- | ----- |
| > | Greater than |
| >= | Greater than equal to |
| < | Less than |
| <= | Less than equal to |
| == | Equal equal to |
| != | Not equal to |

#### Logical Operators

| Operators | Name |
| ----- | ----- |
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

#### Bitwise Operators

Used to perform bit-level operations

| Operators | Name |
| ----- | ----- |
| & | Bitwise AND |
| \| | Bitwise OR |
| ~ | Bitwise NOT |
| << | Left-shift operator |
| >> | Right-shift operator |
| ^ | Exclusive OR |

__Note:__
- Left-shift operator shifts all the bits to the left hand side and the space remained at the right hand side is filled with a _0_
- Left-shift operator is similar to _division by 2_
- Right-shift operator shifts all the bits to the right-hand side and the space remained at the left hand side is filled with a _0_
- Right-shift operator is similar to _multiplication by 2_

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

| A | ~A |
| - | - |
| 0 | 1 |
| 1 | 0 |

| A | B | A ^ B |
| - | - | - |
| 0 | 0 | 0 |
| 0 | 1 | 1 |
| 1 | 0 | 1 |
| 1 | 1 | 0 |

#### Ternary Operator

```
condition ? Statement 1 : Statement 2
```

- It is a shortform of using if-else statement with single condition check.
- If the condition is _True_, Statement 1 will be executed and if it is _False_, Statement 2 will be executed
- Nested ternary operators can also be used for using multiple conditions, but that is not advisable.

#### Operator Precedence

| Priority | Operators |
| ----- | ----- |
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