### Variable, Scope and Lifetime

Variable is the named memory location used to store data whose value changes during execution of the program

```cpp
int x = 10;
```

Here, `int` is the data type, `x` is the name for the memory location and 10 is the value stored in that memory location in bit format

#### Scope

- Region of a program where a variable can be accessed
- Scope tells where a variable is visible and where it can and cannot be accessed
- Scope helps prevent name conflicts, organize code better, limit accidental use of variables and makes debugging easier

#### Types of Scope

1. Local Scope

    Variable is declared inside a block or function

    ```cpp
    void fun() {
        int x = 20;
        std::cout << x;
    }
    ```

1. Global Scope 

    Variable is declared outside all the functions

    ```cpp
    int x = 20;

    void fun() {
        std::cout << x;
    }
    ```

1. Block Scope

    Variable declared within the curly braces _{}_ 

    ```cpp
    if(true) {
        int y = 10;
        std::cout << y;
    }
    ```

1. Function Scope

    Variable declared inside functions are not visible outside the functions

__Note:__

Local variable can hide a global variable with the same name

```cpp
int x = 10;         // Global variable

int main() {
    int x = 20;     // Local variable

    std::cout << x;
}
```

#### Lifetime

Lifetime describes how long the variable exists in the memory

#### Local vs Global Variable

| Factors | Local Variable | Global Variable |
| ----- | ----- | ---- |
| Declaration | Function or Block | Outside all functions |
| Scope | Limited | Whole file or accessible across functions |
| Lifetime | Until block or function ends | Entire program |
| Default value | Garbage value if uninitialized | Zero-initialized |

_Garbage value is the unitialized or unpredictable value_

---