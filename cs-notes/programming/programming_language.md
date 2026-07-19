### Programming Languages

#### Types of programming languages

Classification based on level of abstraction from hardware

1. Low-level Language OR Machine Language OR 1GL
1. Assembly Language OR 2GL
1. High-level Language OR 3GL

_abstrction - hiding complex realities of computers components behind software interface_

#### Machine Language

- First generation language (1GL)
- Consists of binary instructions (0s and 1s) that are directly understood and executed by the CPU

    #### Characteristics

    - Written in binary
    - Executed directly by the CPU
    - No translator required
    - Very fast execution
    - Difficult for humans to read and write
    - Hardware dependent

    #### Advantages

    - Fastest execution
    - No translation overhead
    - Maximum hardware control

    #### Disadvantages

    - Extremely difficult for humans to read and write
    - Difficult to test, debug and maintain
    - Not portable

#### Assembly Language

- Second generation language (2GL)
- Instead of binary numbers, mnemonic instructions _(symbolic instruction)_ were used
- Low-level programming language
- Must be translated into machine language by using an assembler

    #### Characteristics

    - Uses mnemonic
    - Easier than machine language
    - Hardware dependent
    - Requires an assembler
    - Provides direct access to hardware

    #### Advantages

    - Easier than binary
    - Faster execution
    - Efficient memory usage
    - Useful for embedded systems and device drivers

    #### Disadvantages

    - Machine dependent
    - Difficult for large software projects
    - Less readable than high-level language

#### High-Level Language

- Third generation language (3GL)
- Uses English-like syntax and abstracts away hardware details making programs easier to read and write

    _abstracts away hardware details - hiding complex low-level physical workings of a computer from software developers_

    #### Characteristics

    - Human readable
    - Portable
    - Easier to debug and maintain
    - Machine independent
    - Requires language processors

    #### Advantages

    - Easy to learn
    - Faster development
    - Better readability
    - Easier maintenance
    - Large standard libraries

    #### Disadvantages

    - Slightly slower than low-level languages
    - Less direct control over hardware

#### Types of High-Level Programming Languages

1. Procedural Programming Language

    - Programs are organized as procedures or functions
    - C, Pascal

    _C is middle-level language or procedural language because it offers low-level features like pointers and direct memory access_

1. Object-Oriented Programming Language

    - Progrms are organized as objects and classes
    - C++, Java, C#

1. Functional Programming Language

    - Programs built using functions and immutable data
    - New variables are created for updating original variable, original values remain intact
    - Haskel, Lisp, F#

1. Scripting Programming Language

    - Used for automation and web development
    - Often interpreted
    - Python, JavaScript, PHP, Ruby

    _Python is scripting + high-level general purpose language_

1. Logic Programming Languages

    - Programs are written using logic and facts
    - Prolog

### Programming Paradigms

- Style or approach to programming
- Not a programming language but a tool for programming

#### Different Programming Paradigms

1. Imperative Programming

    - Focuses on how a task should be performed by giving instructions to the computers
    - C, C++, Java

    #### Types

    1. Procedural Programming

        - Program divided into procedures or functions
        - Program &rarr; Functions &rarr; Data
        - C, Pascal

    1. Object-Oriented Programming

        - Program organized around objects and classes
        - Program &rarr; Objects &rarr; Data + Methods
        - C++, Java, Python

1. Declarative Programming

    - Focuses and what results to be produced instead of describing every execution step

    #### Types

    1. Functional Programming
        - Uses function to build programs
        - Input &rarr; Functions &rarr; Output
    
    1. Logic Programming

        - Uses facts and rules for writing a program
        - Facts / Rules &rarr; Inference Engine &rarr; Answers

#### Examples

| Language | Programming Paradigm |
| ----- | ----- | 
| C | Procedural |
| C++ | Procedural, Object-Oriented, Generic |
| Python | Procedural, Object-Oriented, Functional |
| Java | Object-Oriented, Functional |

---