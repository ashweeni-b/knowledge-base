### Functions

- Way to break the code into chunks for reusability
- Reusable block of code which performs a particular task
- Called by programmer _n_ number of times
- Without functions program can become too lengthy, difficult to read and debug and there are chances of repetitive code blocks

#### Basic Syntax of a Function

```cpp
// Function Declaration
return_type function_name(parameters);

// Function Definition
return_type function_name(parameters) {
    // Body of function

    return value;
}

// Function Call
int main() {
    function_name(arguments);
}
```

- Function declaration/prototype - Informs compiler about the function
- Function definition - Contains actual implementation or instruction
- Function call - Informs compiler to execute the function

#### Why use functions?

- To avoid rewriting the same logic again and again
- To keep track of what we are doing in a program
- To test and check logic independently

#### Example of a Function

```cpp
// Function Prototype
void printHello(); 

int main() {
    // Function Call
    printHello();   
}

// Function Definition
void printHello() {
    printf("Hello!!")
}
```

#### Execution of a function

Execution of a function is done using the __Call Stack__

Before execution of program, <br />
_Program pointer_ - main() <br />
_Call Stack_ - main()

During function call, <br />
_Program pointer_ - main() &rarr; function() <br />
_Call Stack_ - main() | function()

After function execution, <br />
_Program pointer_ - main() &rarr; function() &rarr; main() <br />
_Call Stack_ - main()

#### Types of Functions

1. Library functions

    - Commonly required functions grouped together in a library file on the disk
    - Examples include _printf()_, _scanf()_, _strlen()_, etc.

1. User defined functions

    Functions declared and defined by the user

#### Types of User defined functions

1. No argument and no return value

    ```cpp
    void greet() {
        std::cout << "Hello!!";
    }
    ```

1. Argument but no return value

    ```cpp
    void greet(string name) {
        std::cout << name;
    }
    ```
1. No argument but has a return value

    ```cpp
    void getNumber() {
        return 10;
    }
    ```
1. Argument and has a return value

    ```cpp
    int add(int a, int b) {
        return a + b;
    }
    ```

#### Advantages of Functions

- Code reusability
- Modular programming
- Easier debugging
- Easier maintenance
- Better readability
- Team collaboration

---