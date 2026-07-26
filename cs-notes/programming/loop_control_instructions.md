### Loop Control Instructions

1. while loop 

    ```cpp
    // initialization
    while (condition) {
        // Code if condition is True
        // Updation of loop counter
    }
    ```

    - If the condition never becomes false, the loop never terminates and so an infinte loop is formed
    - Loop counter or variable can be integer or floating-point number

1. do - while loop 

    ```cpp
    // initialization
    do {
        // Code if condition is True
        // Updation of loop counter
    } while (condition);
    ```

    The code executes atleast once and then the condition is checked

1. for loop

    ```cpp
    for(initialization; condition; updation) {
        // Code if condition is True
    }
    ```

    __Note:__

    ```cpp
    for(int i = 1; i <= 5; i++); {
        std::cout << "Hello World";
    }
    ```

    In the case above, compiler considers that the for loop is empty and moves to the next code block and _"Hello World"_ executes only once because of the semi-colon after the for loop.

#### Break and Continue

1. Break statement

    - Used to exit the loop irrespective of whether the condition is true or false
    - Whenever a break is encountered inside the loop, control goes outside the loop

1. Continue statement

    - Used to immediately move to the next iteration of the loop
    - Control is taken to the next iteration thus skipping everything below "continue" inside the loop for that iteration

---