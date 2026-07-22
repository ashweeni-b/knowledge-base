### Tokens

Smallest meaningful unit of a program recognized by the compiler during lexical analysis

#### Types of Tokens

1. Keywords
1. Identifiers
1. Constants
1. Operators
1. String Literals
1. Special Symbols (Separators/Punctuators)

#### Keywords

Reserved words with predefined meanings 

##### Keywords in C

<table>
    <tr>
        <td> auto </td>
        <td> double </td>
        <td> int </td>
        <td> struct </td>
    </tr>
    <tr>
        <td> break </td>
        <td> long </td>
        <td> else </td>
        <td> switch </td>
    </tr>
    <tr>
        <td> case </td>
        <td> return </td>
        <td> enum </td>
        <td> typedef </td>
    </tr>
    <tr>
        <td> char </td>
        <td> register </td>
        <td> extern </td>
        <td> union </td>
    </tr>
    <tr>
        <td> const </td>
        <td> short </td>
        <td> float </td>
        <td> unsigned </td>
    </tr>
    <tr>
        <td> continue </td>
        <td> signed </td>
        <td> for </td>
        <td> void </td>
    </tr>
    <tr>
        <td> default </td>
        <td> sizeof </td>
        <td> goto </td>
        <td> volatile </td>
    </tr>
    <tr>
        <td> do </td>
        <td> static </td>
        <td> if </td>
        <td> while </td>
    </tr>
<table>

##### Keywords in C++

C++ introduced many new keywords because it supports OOP and Generic Programming

<table>
    <tr>
        <td> int </td>
        <td> float </td>
        <td> double </td>
        <td> char </td>
        <td> bool </td>
        <td> void </td>
    </tr>
    <tr>
        <td> long </td>
        <td> short </td>
        <td> signed </td>
        <td> unsigned </td>
        <td> auto </td>
        <td> if </td>
    </tr>
    <tr>
        <td> else </td>
        <td> switch </td>
        <td> case </td>
        <td> default </td>
        <td> for </td>
        <td> while </td>
    </tr>
    <tr>
        <td> do </td>
        <td> break </td>
        <td> continue </td>
        <td> goto </td>
        <td> return </td>
        <td> class </td>
    </tr>
    <tr>
        <td> struct </td>
        <td> public </td>
        <td> private </td>
        <td> protected </td>
        <td> virtual </td>
        <td> friend </td>
    </tr>
    <tr>
        <td> this </td>
        <td> new </td>
        <td> delete </td>
        <td> inline </td>
        <td> try </td>
        <td> catch </td>
    </tr>
    <tr>
        <td> throw </td>
        <td> static </td>
        <td> extern </td>
        <td> register </td>
        <td> const </td>
        <td> sizeof </td>
    </tr>
    <>
        <td> typedef </td>
        <td> template </td>
        <td> enum </td>
        <td> union </td>
        <td>  </td>
        <td>  </td>
    </tr>
<table>

#### Identifiers

- Identifiers are user-defined names
- Identifiers can represent
    - Variables
    - Classes
    - Functions
    - Objects
    - Arrays
    - Structures
    - Namespaces
- Rules for an identifier
    - Can start with alphabet or underscore
    - Cannot start with a digit
    - Cannot contain commas and spaces
    - Cannot be a keyword
    - Is case-sensitive

```cpp
// Variables
int age = 20;

// Functions
int add(int a, int b);

// Classes
class Student {
    string name;
    int age;
}

// Objects
Student s1;

// Arrays
int arr = {1, 2, 3, 4, 5};

// Structures
struct Employee {
    int id;
    string name;
    float salary;
}

// Namespaces
using namespace std;
```

#### Constants (Literals)

- Constants are fixed values
- Types of Constants    
    - Integer constants
    - Floating-point constants
    - Character constants
    - String literals
    - Boolean literals

```cpp
// Integer
const int age = 20;

// Floating-point
const float pi = 3.14;

// Character
const char = '*';

// String
const string name = "Jacob";

// Boolean
const bool isSquare = true;
```

#### String Literals

Sequence of characters enclosed in double quotes

```cpp
string name = "Anna";
```

#### Operators

| Operator | Name |
| ----- | ----- |
| + | Addition |
| < | Less than |
| \|\| | Logical OR |
| ! | NOT |

These are some of the examples of operators

#### Special Symbols (Separators/Punctuators)

- These symbols separate or organize program elemetns
- ; , () {} [] * : :: are some of the special symbols

---