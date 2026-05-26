### Dynamic Memory Allocation

- Since C is a low level language, it allows memory management
- Dynamic Memory Allocation is a way to allocate memory to a data structure during runtime using functions

#### Functions for Dynamic Memory Allocation

All the functions are present in the `<stdlib.h>` library function

1. `malloc()`
    - Stands for memory allocation
    - Take number of bytes to be allocated as an input and returns a pointer of type void
    - Since it is a void pointer, it is type-casted to the required data type
    
    ```c
    // Stores integer values in array
    int* arr;

    arr = (int*) malloc(n * sizeof(int));

    // Stores floating values in array
    float* arr;

    arr = (float*) malloc(n * sizeof(float));
    ```

    - The expression returns a null pointer if the memory cannot be allocated
    - All the values are initialized with garbage values

1. `calloc()`

    - Stands for continous allocation
    - Similar to `malloc()` but it initializes each memory block with the value of 0

    ```c
    int* arr;

    arr = (int*) calloc(n, sizeof(int));
    ```

    - Allows contiguous memory allocation for `n` values
    - If the space is not sufficient, memory allocation fails and a NULL pointer is returned

1. `free()`

    - Used to deallocate the memory
    - Memory allocated using `calloc()` and `malloc()` is not deallocated automatically

    ```c
    // Memory Allocation

    free(arr)
    ```

1. `realloc()`

    - Sometimes the dynamically allocated memory is insufficient or more than required
    - Used to allocate memory of new size using the previous pointer and size

    ```c
    int* arr;

    // Allocation of memory
    arr = (int*) malloc(5 * sizeof(int));

    // Reallocation of memory
    arr = (int*) malloc(10 * sizeof(int));
    ```

---