### Pointers

A variable that stores the address of another variable

#### The Address of (&) operator

- Used to obtain the address of a given variable
- Pointer variable denoted by the `int*` variable
- Format specifier `%p` or `%u` is used to print the address of the variable
- `%p` is the pointer memory address in the hexadecimal format
- `%u` is the pointer memory address in the unsigned integer format

#### The Value at address (*) operator

Used to obtain the value at a given memory address

#### Pointer Visualization

![Pointer to Pointer](./assets/Pointer_Visualization.png)

Here, the variable `i` is the integer variable which stores value, `j` is the pointer variable which stores the address of variable `i` and `k` is the pointer to pointer variable which stores the address of variable `j`.

#### Declaration of Pointer

Pointers can be of integer type, character type or floating-point type

```c
#include <stdio.h>

int main() {
    // Declaration of variable
    int i = 42;

    // Declaration of pointer
    int* j = &i;

    // Declaration of pointer to pointer
    int** k = &j;

    printf("Value of i: %d\n", i);
    printf("Value of i using pointer: %d\n", *j);
    printf("Value of i using pointer: %d\n", *(&i));
    printf("Value of i using pointer to pointer: %d\n", **k);
    printf("Value of i using pointer to pointer: %d\n", **(&(&i)));
    printf("Address of i: %u\n", &i);
    printf("Address of i using pointer: %u\n", j);
    printf("Address of i using pointer to pointer: %u\n", *k);

    return 0;
}
```

#### Types of Function Calls

1. Call by value
    
    Value of argument is passed to the function

    ```c
    #include <stdio.h>

    int sum(int a, int b);

    int main() {
        int a = 5, b = 5;

        printf("Sum is: %d", sum(a, b));    // Values are passed

        return 0;
    }

    int sum(int a, int b) {
        return a + b;
    }
    ```

1. Call by reference
    
    Address of argument is passed to the function

    ```c
    #include <stdio.h>

    int sum(int* a, int* b);

    int main() {
        int a = 5, b = 5;

        printf("Sum is: %d", sum(&a, &b));    // Addresses are passed

        return 0;
    }

    int sum(int* a, int* b) {
        return *a + *b;
    }
    ```

#### Pointer Arithmetic

- A pointer can be incremented to point to the next memory location of that type

```c
// Integer pointer
int i = 32;
int *a = &i;        // a = 87994
a++;                // a = 87998

// Character pointer
char b = 'A';
char *c = &b;        // a = 87994
c++;                 // a = 87995

// Floating pointer
float m = 1.5;
float *n = &m;       // a = 87994
n++;                 // a = 87998
```

- Following operations can be performed on a pointer:
    1. Addition of a number to a pointer
    1. Subtraction of a number to a pointer
    1. Subraction of one pointer from another
    1. Comparison of two pointer variables
- Pointer arithmetic can be performed only on same type of pointers
- Addition and subtraction with pointers denotes that the memory address gets updated according to the pointer type (depending on the type of the data)

---