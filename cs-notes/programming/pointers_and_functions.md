### Pointers and Functions

Pointers can be passed to functions

#### Pass by value
    
Value of argument is passed to the function. Original value remains unchanged.

```cpp
#include <iostream>

int sum(int a, int b);

int main() {
    int a = 5, b = 5;

    std::cout << "Sum is: " << sum(a, b) << std::endl;    // Values are passed

    return 0;
}

int sum(int a, int b) {
    return a + b;
}
```

#### Pass by reference
    
Address of argument is passed to the function. Original values gets modified.

```cpp
#include <iostream>

int sum(int *a, int *b);

int main() {
    int a = 5, b = 5;

    std::cout << "Sum is: " << sum(&a, &b) << std::endl;    // Values are passed

    return 0;
}

int sum(int *a, int *b) {
    return *a + *b;
}
```

#### Function Pointer

Pointer pointing to the address of the function

```cpp
// Function
int sum(int a, int b) {
    return a + b;
}

// Function Pointer
int (*ptr)(int, int) = add;

// Calling function
ptr(5,3);
```

`sum()` has memory address of 5000 and ptr points to memory address 5000

---