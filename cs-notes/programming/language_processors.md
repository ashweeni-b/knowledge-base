### Language Processors

- Codes are written in human-readable language
- CPU only understand machine instructions (binary instructions)
- Language Processors translates human-readable language into machine language

    Source Code &rarr; Language Processors &rarr; Machine Code

- System software that translates a program written in one language (high-level or assembly) into machine language or another form that a computer can understand

#### Types of Language Processors

1. Compilers - translates entire code block
1. Interpreters - translates code line by line
1. Assemblers - translates assembly code

#### Compilers

- Converts entire source code into machine code before execution of the program

    Source Code &rarr; Compiler &rarr; Machine/Object Code &rarr; Executable File &rarr; Run &rarr; Output

- Examples - C, C++, Go, Rust

#### Characteristics of Compilers

1. Translates the entire program at once
1. Produces an executable file
1. Reports compilation errors together
1. Faster execution after compilation

#### Interpreters

- Translates and executes the program one statement at a time
- Does not usually generates a separate executable 

    Source Code &rarr; Interpreter &rarr; Translate one line &rarr; Execute &rarr; Translates another line &rarr; Execute &rarr; ...... &rarr; Output

    Translation and exeuction continues until all the program statements are executed

- Examples - Python, JavaScript, Ruby

#### Characteristics of Interpreters

1. Executes line by line
1. No separate executable file in the usual workflow
1. Stops when it encounters an error
1. Slower execution because translation occurs during execution

#### Assemblers

- Converts assembly language into machine code

    Assembly Code &rarr; Assembler &rarr; Machine Code

- Examples - NASM, MASM, GAS

#### Characteristics of Assembers

1. Converts assembly language into machine code
1. Very fast
1. Used in embedded systems, firmware, and low-level programming

---