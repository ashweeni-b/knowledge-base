### Structures

- Array and strings store similar data types
- Structures store dissimilar data types into a single variable
- Collection of variables of different types under a single variable
- Defined outside the `main()` function for better understanding

#### Example

```c
struct employee_data {
    int code;
    float salary;
    char name[20];
};
```

#### Why Use Structures?

Structures keep the data organized and makes data management easy for the programmer

#### Array of Structures

```c
struct employee_data employee[20];
```

While creating members of structures in the `main()` function, an array of members can be created and the members can be accessed using the array

#### Initializing Structures

```c
struct employee_data emp1 = {473, 45000.00, "Jacob"};
```

It assigns the code 473, salary as 45000.00 and the name Jacob to emp1

```c
struct employee_data emp2 = {0};
```

It assigns the code 0, salary as 0.0 and name as "0" to emp2

#### Structures in Memory

employee_data instances are stored in contiguous memory location adjacent to each other <br />

![Structures in Memory](./assets/Structure_in_Memory.png)

#### Pointer to Structures

```c
struct employee_data emp1;
struct empoyee_data *ptr;

// emp1 is assigned with a pointer
ptr = &emp1;

// Accessing emp1 to pointer
printf("%d %f %s", (*ptr).code, (*ptr).salary, (*ptr).name);
```

#### The Arrow (->) Operator

Instead of writing `(*ptr).code` we can use arrow operator to access structure properties

```c
printf("%d %f %s", (*ptr).code, (*ptr).salary, (*ptr).name);
printf("%d %f %s", ptr -> code, ptr -> salary, ptr -> name);
```

#### Passing Structure to a Function

```c
// Function declaration
void show_data(struct employee_data employee1);

// Function call
show_data(emp1);

// Function definition
void show_data(struct employee_data employee1) {
    printf("%d %f %s", employee1.code, employee1.salary, employee1.name);
}
```

#### Typedef Keyword

- Used to create an alias of structure
- Basically, an alias of any data type can be created using `typedef` keyword

```c
typedef struct employee_data {
    int code;
    float salary;
    char name[20];
} employee;

int main() {
    employee emp1, emp2;    // emp1 and emp2 has data type of structure

    // Code
}
```

OR

```c
struct employee_data {
    int code;
    float salary;
    char name[20];
};

int main() {
    typedef struct employee_data employee;

    employee emp1, emp2;    // emp1 and emp2 has data type of structure

    // Code
}
```

---