### Conditional Instructions

1. if statement 

    ```cpp
    if (condition) {
        // Code if condition is True
    }
    ```

1. if - else statement 

    ```cpp
    if (condition) {
        // Code if condition is True
    } else {
        // Code if condition is False
    }
    ```

1. if - else if statement

    ```cpp
    if(condition1) {
        // Code if condition1 is True
    } else if (condition2) {
        // Code if condition2 is True
    }
    ```

1. if - else if - else statement

    ```cpp
    if (condition1) {
        // Code if condition1 is True
    } else if (condition2) {
        // Code if condition2 is True
    } else {
        // Code if condition is False
    }
    ```

    - The else statement mandatorily requires if statement but not vice-versa
    - These loops can also be nested within each other

1. switch statement

    - Executes different blocks of code based on value of an expression
    - Used when a choice is need to be made between multiple alternatives for a given variable

    ```cpp
    switch(expression) {
        case value1:
            // Code if value1
            break;

        case value2:
            // Code if value2
            break;

        case value3:
            // Code if value3
            break;

        .....

        default:
            // Code
    }
    ```

#### Conditions pertaining switch statement

1. Cases within switch statement can be written in any order and not necessarily ascending or descending
1. The expressions can have data type as int, char or enum but not float or string
1. Case values must be unique and not repetitive
1. Conditions are not checked as cases
1. Fall Through Behaviour

    Each case statement should have break within it else all the code within the cases after the first true gets executed
1. A switch can occur within another but in practice it is rarely done

---