### File I/O

- The random access memory is volatile and its content is lost once the program terminates
- In order to persist the data forever we use files
- A file is data stored in a storage device
- A C program can talk to file by reading content from it and writing content to it

#### FILE Pointer

- A file is a structure which needs to be created for opening the files
- A FILE pointer is a pointer to this structure of the file
- FILE pointer is needed for communication between the file and the program

```c
FILE* ptr;

ptr = fopen("filename.ext", "mode");
```
The filename and the mode in which the file needs to be opened are the parameters to the fopen function

#### File Opening Modes in C

| Mode | Meaning |
| --- | --- |
| `r` | Open for reading |
| `rb` | Open for reading in binary |
| `w` | Open for writing <br /> If the file exists, the contents will be overwritten |
| `wb` | Open for writing in binary |
| `a` | Open for append <br /> If the file does not exist, it will be created |

#### Types of Files

Primarily, there are two types of files:

1. Text Files - .txt, .c
1. Binary Files - .jpg, .dat

#### Reading a File

```c
FILE* ptr;

ptr = fopen("numbers.txt", "r");    // numbers.txt file is created in the root folder

int num;

fscanf(ptr, "%d", &num);

printf("Number is: %d", num);
```

#### Writing to a File

```c
FILE* ptr;

ptr = fopen("numbers.txt", "w");    // numbers.txt file is created in the root folder

int num 40;

fprintf(ptr, "%d", num);
```

If there are any content in the file then it will be overwritten

#### Closing the File

It is very important to close the file after read or write.

```c
// File Working

fclose(ptr)
```
Tells the compiler that the working with the file is doen and it could be released

#### fgetc() and fputc()

`fgetc()` - Reads a character from a file. Used in read mode
`fputc()` - Writes a character to a file. Used in write mode

```c
FILE *ptr;

ptr = fopen("name.txt", "r");

char ch = fgetc(ptr);

printf("%c", ch);

fclose(ptr);

ptr = fopen("name.txt", "w");

char ch = 'A';

fputc(ch, ptr);
```

### EOF - End of a File

`fgetc()` returns EOF when all characters from a file have been read

```c
FILE *ptr

ptr = fopen("name.txt", "r");

while(1) {
    char ch = fgetc(ptr);

    if(ch == EOF) {
        break;
    }

    printf("%c", ch);
}
```

---