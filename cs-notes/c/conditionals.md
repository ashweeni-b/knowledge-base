### Conditional Instructions

Conditions are met and instructions are executed

#### Types of Conditional Instructions

1. if statement 

    ```c
    if (condition) {
        // Code if condition is True
    }
    ```

1. if - else statement 

    ```c
    if (condition) {
        // Code if condition is True
    } else {
        // Code if condition is False
    }
    ```

1. if - else if - else statement

    ```c
    if (condition1) {
        // Code if condition1 is True
    } else if (condition2) {
        // Code if condition2 is True
    } else {
        // Code if condition is False
    }
    ```

    - The else statement mandatorily requires if statement but not vice-versa
    - Multiple else-if statements can be written within the conditional instructions
    - These loops can also be nested within each other

1. switch statement

    Used when a choice is need to be made between multiple alternatives for a given variable

    ```c
    switch(expression) {
        case c1:
            // Code
            break;

        case c2:
            // Code
            break;

        .....

        default:
            // Code
    }
    ```

    - Cases within switch statement can be written in any order and not necessarily ascending or descending
    - `char` values are allowed in cases as their values can be evaluated to integer
    - A switch can occur within another but in practice it is rarely done

---