A programming language **acts as a bridge** between what **humans understand** and what a **computer understands**

Programs are sets of instructions that enable a computer to perform specific tasks.
Programs can be written in high-level or low-level languages, according to the requirements of the user.
High-Level languages => Assembly languages => Machine code => Binary code -> to computer machine



- A high-level programming language uses **English-like statements** to allow users to program with easy to use code
- High-level languages allow for clear **debugging** and once programs are created they are **easier to maintain**
- High level languages were needed due to the **development of processor speeds** and the **increase in memory capacity**
- **One instruction** translates into **many machine code instructions**
- **Needs to be translated** into machine code for the computer to be able to execute it
High level languages enable a programmer to write programs for a computer without knowledge of the hardware and instruction sets of that computer.
Same programming concepts can be applied to different high-level languages.
They are considered portable, you can write the program on one computer, and run it on a different computer.


- A low-level language is a programming language that **directly translates to machine code** understood by the processor
- Low-level languages allow **direct control over hardware** components such as **memory** and **registers**
- These languages are written for **specific processors** to ensure they embed the correct machine architecture
Low level languages are related to the hardware architecture and its instruction set. Machine code, binary instructions that are understandable by the computer. Assembly language needs to be converted to machine code.
Machine code is non portable, the same code may not run on a different computer.
Assembly language uses **mnemonics** to represent code.
- **LDA Load** - this will ensure a value is added to the accumulator
- **ADD Addition** - this will add the value input or loaded from memory to the value in the accumulator
- **STO, Store** - stores the value in the accumulator in RAM




High level language
- easier for humans to understand, read, write, amend, debug
- portable
- must be converted into a low-level language before it can be run
- one statement can represent many low-level instructions
- cannot directly manipulate hardware
Low level language
- more difficult for humans
- not portable, machine dependent
- does not need converting, assembly language must be assembled before execution, but this is faster than from a high-level language
- several instructions are needed for each high-level language statement
- can directly manipulate the harder ex. memory. this can make the program more efficient in terms of speed and memory usage.



---
Assembly language
is used to manipulate and make use of computer hardware
instructions are different for different types of machines
it does not take up much space of primary memory and performs its task quickly
- Programmers use assembly language for the following reasons:
    - Need to make use of **specific hardware** or parts of the hardware
    - To complete **specific machine dependent** instructions
    - To ensure that too much space **is not taken up in RAM**
    - To ensure code can completed much **faster**

Code to add two numbers:
`MOV AX, 22h` move the hex number 22 to register AX
`ADD AX, 15h` add the number in the register AX with hex number 15
`HLT` stop


- **LDA Load** - this will ensure a value is added to the accumulator
- **ADD Addition** - this will add the value input or loaded from memory to the value in the accumulator
- **STO, Store** - stores the value in the accumulator in RAM

Assembler
an assembler is a computer program that translates assembly language programs into machine code so it can be used by the computer to perform the task. 
Once assembled once, it can be used without re-assembly.

- A **mnemonic** is received by the computer and it is looked up within a specific table
- An **assembler** is needed to check the word so that it can be converted into machine code
- If a match from the word is found e.g. STO the word is replaced with the relevant binary code to match that sequence




Recall

Little Question:
CLI stands for Command Line Interface
GUI stands for Graphical User Interface


# task 1
Computers require different programming languages because a computer cannot read human languages such as our alphabet. They can only read and comprehend binary code. So, a high-level language must be converted into a low-level language for the computer to understand.

# task 2
High-level languages
- easier for humans to read, write, debug
- one statement can represent a lot of lines of low-level languages
- they are portable

- must be converted to run
- cannot directly manipulate hardware
- there are several different languages needed to do different aspects of computer tasks.

Low-level languages
- can directly manipulate hardware
- does not need converting
- must be assembled before execution, but this is faster than high-level languages conversion

- more difficult to read, write, debug
- a lot of statements are needed to represent one statement from a high-level language
- they are not portable, they are machine-dependent


# task 3
A programmer should choose a low-level language if they want more granular control over the computer's execution, it provides direct control over hardware and resources. They can make specific programs for specific architecture of a specific computer.

# plenary
A high-level language uses human-style words as instructions.



review learning
www i understand the advantages and disadvantages of both high level and low level languages
ebi remember the definitions and learn more about mnemonics







---
recall
little question
High level languages use human styled code to write programs. They have to be turned into machine code to run.
Low level languages is a programming language that directly translates to machine code understood by the processor. They are harder to write and longer to write than high level languages. They can directly manipulate machine hardware.

# Task 1
Assembly language is used to make use of and manipulate computer hardware. It uses mnemonics and then machine code. You have to write several statements for a single high level programming language statement, but it performs its task quickly and does not take up a lot of primary memory.

# task 2
Mnemonics are 1 to 1 instructions that are converted to binary.
`INP` - input, copies the value from the 'in box' onto the accumulator
`STA` - store, stores the contents of the accumulator to the given address
`ADD` - add, adds the contents of the address given to the accumulator
`OUT` - output, copies the value from the accumulator to the 'out box'
`HLT` - halt, stops the program

# task 3
An assembler first takes the mnemonics and looks it up, if a match is found, the word is replaced with the relevant library machine code to match that sequence. 

# plenary
A high level language is translated to assembly language.
Assembly language is assembled into machine code.
Machine code can be read by the CPU and then be processed and executed

High-level language => assembly language => machine code  --> CPU

review learning
www
	understood some assembly language is written and assembled
ebi
	learn some mnemonics and how to point to memory register addresses