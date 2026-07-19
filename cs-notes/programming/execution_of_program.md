### Execution of a Program

- Process of translation of source code into machine code, loding the code into the memory and execution of the machine code

    Problem &rarr; Algorithm &rarr; Source Code &rarr; Language Processors &rarr; Machine Code &rarr; Loader &rarr; RAM &rarr; CPU &rarr; Output

#### Flow of Execution of a Program

Problem Definition &rarr; Alogrithm &rarr; Writing source Code &rarr; Translation &rarr; Linking &rarr; Executable File &rarr; Loading &rarr; CPU Execution &rarr; Output

- The source code is preprocessed before giving it to the compiler
- The header files gets combined with the source code and it contains prototypes and directives. The source code is then given to the compiler
- The compiler translates the human-readable code into assembly code
- The assembly code is then given to the assembler for its translation into machine code
- The assembler generates the _.obj_ object file
- The object file is passed through the linker for linking of library functions
- An executable file is created by the linker
- The executable is then passed to the loader
- OS loads the executable into the RAM and during loading memory is allocated, program sections are loaded and execution is prepared
- After successful loading, the CPU executes the instructions
- CPU follows Fetch &rarr; Decode &rarr; Execute cycle until the program completely executes
- Fetch means next instruction is fetched from memory, Decode means the meaning of the instructions is determined by the control unit and Execute means the ALU, registers or the other CPU components performs required operations
- After successful CPU cycles the output is displayed

#### Execution of Compiled Languages

Source Code &rarr; Compiler &rarr; Assembly &rarr; Assembler &rarr; Object File &rarr; Linker &rarr; Executable &rarr; Loader &rarr; CPU &rarr; Output

#### Execution of Interpreted Languages

Source Code &rarr; Interpreter &rarr; Translation &rarr; Execution &rarr; Output

#### Execution of Assebly Languages

Assembly Code &rarr; Assembler &rarr; Machine Code &rarr; Loader &rarr; CPU &rarr; Output

---