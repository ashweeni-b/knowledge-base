### Structure of a program

#### C

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
    - Include the library functions required for the execution of the program
    - _stdio.h_ has scanf() and printf() functions

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

#### C++

```cpp
#include <iostream>
using namespace std;

int main() {
    cout << "Hello World" << endl;
    return 0;
}
```

The program has multiple parts and they are:

1. Header File

    ```cpp
    #include <iostream>
    ```
    
    - _#include_ is the preprocessor directive and _iostream_ is the header file. <br />
    - Include the library functions required for the execution of the program
    - _iostream_ has cin (input stream), cout (output stream), cerr (error stream) and clog (log stream) functions

1. Namespace Definition

    ```cpp
    using namespace std;
    ```

    Allows programmer to use the standard library names without writing _std::_ everytime

1. Main Function

    ```cpp
    int main() { 
        // Code
    }
    ```

    - _main()_ is the starting point of the exeuction of the program. <br />
    - Execution occurs line by line since the program passes through the compilation process. <br />
    - _main()_ function has the return type of integer. <br />
    - It means that the function will return an integer value after successful execution of the program to the operating system. <br />
    - _{}_ denotes the block of code to be executed and also the scope of the code.

1. Body of the code

    ```cpp
     cout << "Hello World" << endl;
    ```

    - _cout_ is the library function which displays the output to the console
    - _endl_ provides newline to the console
    - _;_ is the statement terminator

1. Return statement

    ```cpp
    return 0;
    ```

    - _return_ is a keyword which denotes the ending point of the execution of the program
    - _0_ here demonstrates that the code is sucessfully executed with no or zero errors
    - Any non-zero value denotes unsuccessful execution of the program

---