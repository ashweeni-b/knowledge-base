### Structure of a C program

Consider the following example of a C program to print Hello World as the output.

```c
#include <stdio.h>

int main() {
    printf("Hello World!");

    return 0;
}
```

The program has multiple parts and they are:

1. Header File

    ```c
    #include <stdio.h>
    ```
    
    - _#include_ is the preprocessor directive and _stdio.h_ is the header file. <br />
    - Include the functions required for the execution of the program

1. Main Function

    ```c
    int main() { 
        // Code
    }
    ```

    - _main()_ is the starting point of the exeuction of the program. <br />
    - Execution occurs line by line since the program passes through the compilation process. <br />
    - _main()_ function has the return type of integer. <br />
    - It means that the function will return an integer value after successful execution of the program. <br />
    - _{}_ denotes the block of code to be executed.

1. Body of the code

    ```c
    printf("Hello World");
    ```

    - _printf()_ is the function which displays the output to the console
    - _;_ is the statement terminator

1. Return statement

    ```c
    return 0;
    ```

    - _return_ is a keyword which denotes the ending point of the execution of the program
    - _0_ here demonstrates that the code is sucessfully executed with no or zero errors

#### Boiler Plate Code

```c
#include <stdio.h>

int main() {

    return 0;
}
```

The above code is the boiler plate code in C, which tells that this is the base code and is used in every other C program

---