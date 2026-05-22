### Functions

- Way to break the code into chunks for reusability
- Block of code which performs a particular task

#### Function Declaration

```c
// Function prototype
void printHello(); 

#include <stdio.h>

int main() {
    // Function call
    printHello();   
}

// Function definition
void printHello() {
    printf("Hello!!")
}
```

- Function prototype informs compiler about the function
- Function call instructs the compiler to execute the function's body
- Function definition contains the exact instructions to be executed

The program control flows from ___main() &rarr; function() &rarr; main()___

#### Types of Functions

1. Library functions

    - Commonly required functions grouped together in a library file on the disk
    - Examples include _printf()_, _scanf()_, _strlen()_, etc.

1. User defined functions

    Functions declared and defined by the user

#### Why use Functions?

1. To avoid rewriting the same logic again and again
1. To keep track of what we are doing in a program
1. To test and check logic independently

#### Passing values to Functions

```c
int sum(int a, int b);      // Parameters

#include <stdio.h>

int main() {
    int x = 3, y = 5;

    printf("Sum: %d", sum(x, y));   // Arguments

    return 0;
}

int sum(int a, int b) {
    return a + b;
}
```

The variables passing into the function call are the arguments and the one defined in the function declaration are parameters. Here, _a_ and _b_ are the parameters and _x_ and _y_ are the arguments.

_Note:_ Copy of variables are passed are arguments to the functions.

---