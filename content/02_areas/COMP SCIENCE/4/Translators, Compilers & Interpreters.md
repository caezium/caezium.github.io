### What is a translator?
- A translator is a program that **translates** program **source code** into **machine code** so that it can executed directly by a processor
- **Low-level languages** such as **assembly code** are translated using an **assembler**
- **High-level languages** such as **Python** are translated using a **compiler** or **interpreter**
    
### What is a compiler?
- A compiler translates high-level languages into machine code **all in one go**
- Compilers are generally used when **a program is finished** and has been checked for syntax errors
- Compiled code can be **distributed (creates an executable)** and run **without the need for translation software**
- If compiled code contains any errors, after fixing, it **will need re-compiling**
    
| **Advantages**                        | **Disadvantages**                                |
| ------------------------------------- | ------------------------------------------------ |
| Speed of execution                    | Can be memory intensive                          |
| Optimises the code                    | Difficult to debug                               |
| Original source code will not be seen | Changes mean it must be recompiled               |
|                                       | It is designed solely for one specific processor |

### What is an interpreter?
- An interpreter translates high-level languages into machine code **one line at a time**
- Each line is executed after translation and if **any errors are found**, the **process stops**
- Interpreters are generally used when a program **is being written** in the development stage
- Interpreted code is more **difficult to distribute** as **translation software is needed for it to run**
    

|**Advantages**|**Disadvantages**|
|---|---|
|Stops when it finds a specific **syntax error** in the code|Slower execution|
|Easier to debug|Every time the program is run it has to be translated|
|Require less RAM to process the code|Executed as is, no optimisation|



---
recall
Operating systems have 8 main functions
- Multitasking and memory - using interrupts and managing resources, the OS can decide which processes to run first and because the microprocessor is so fast, it will seem like multiple applications are executing at the same time.
- interface - provides an user interface for human-computer interaction such as a graphical user interface or command line interface
- security - provides security features like a firewall, anti-virus checker, account password protection, file encryption
- file management - allows users to create and manage files and directories
- applications - provides a platform for application software to run on
- handles interrupts - handles the priority of processes and sends the optimized interrupts to allow the computer to run smoothly
- peripherals and devices - translates drivers' data to the computer to manage input and output devices to allow the users to interact with the computer such as using a mouse or printing a PDF
- user accounts - manages different user accounts to allow different access permissions, preferences, and files.

### task 1
interpreters translate high-level languages into machine code one line at a time and runs it straight after. If that line has an error, the interpreter stops and shows the error.
Compilers translates the entire high-level language code file into machine code and generates an executable file that can be distributed easily.


### task 2
interpreters translate high-level languages into machine code one line at a time and runs it straight after. If that line has an error, the interpreter stops and shows the error.
Compilers translates the entire high-level language code file into machine code, errors are pointed out only after the compilation of the program

### task 3
Compilers can be useful to distribute a program after it is done testing and developing. Compilers optimize the code and it is faster to execute without having to be compiled again. Compiled code will also not show their source code, protecting developers intellectual property. 
However, compiled programs are difficult to debug and any changes means that it has to be recompiled. They are also designed for different unique types of processors.
Compilers should be used after the program is done testing and developing, when it is ready to be shared to others.

Interpreters are useful when testing or developing. They can run through the code one line at a time and show you the errors so that you can fix them fast without having to compile the entire file. This makes it easier to maintain and debug. 
However, interpreters are slower at execution and it has to be re-interpreted every time without optimization.
Interpreters should be used when you are in the middle of developing a program.



review learning
www
understood the difference between the terms interpreters and compilers
ebi
remember when and where the errors in the code for each type of translator is reported and checked.