### Type Casting

- Change data type of a variable from one data type to another
- Crucial when different data types are used while performing operation

- Type-casting: <br/>
    - Implicit Type casting
    - Explicit Type casting

#### Implicit Type Casting

- Automatic type conversion
- Compiler automatically converts from one data type to another during operation execution
- Compiler promotes one type to larger type to maintain precision

    char op int &rarr; int <br />
    float op int &rarr; float <br />
    double op int &rarr; double <br />

```cpp
// float gets demoted to int
int d = 6.7;
std::cout << d << std::endl;

// Output: 6
```

```cpp
// int gets promoted to float
float e = 8;
std::cout << e << std::endl;

// Output: 8.0
```

```cpp
// int gets promoted to int
float d = 10 + 15.5;
std::cout << d << std::endl;

// Output: 25.5
```

```cpp
// char gets promoted to int
char ch = 'A' + 1;
std::cout << ch << std::endl;

// Output: 66
```

#### Explicit Type Casting

- Manual type conversion
- Allows to explicitly specify the desired data type during assignment or operation
- Represenation: _(data_type)_

```cpp
// float to int
int a = 8;
float b = 3.5;
float sum = a + (int)b;
std::cout << sum;

// Output: 11
```

```cpp
// double to int
double pi = 3.141592695;
int ipi = (int)pi;
std::cout << ipi;

// Output: 3
```

```cpp
// float to char
float num = 65.35;
char ch = (char)num;
std::cout << ch;

// Output: A
```

---