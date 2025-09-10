```toc
```

# CPU

- a computer system consists of
    - hardware
    - software

### Hardware

- input devices
- **CPU**
- primary memory
- output devices
    - secondary storage

### The role of the central processing unit

1. To **process instructions** and **data** that are input into the computer to enable the output of results
2. carries out the Fetch-Decode and Executes cycle

### Peripherals

- external devices that are connected to a computer to add functionality
- drivers act as the bridge between the peripheral device and the computer's operating system
- e.g. mouse, keyboard

### Microprocessor

- the **integrated circuit on a single chip**
- used to perform logical and arithmetic operations
- can be used in a wide range of devices
- includes CPU but microprocessor includes more (e.g. GPU)

## Von Neumann Architecture

### Features

1. The concept of a **central processing unit**
2. **stored program concept** (memory stores data and instruction)
3. The CPU can access the memory **directly**
4. serially **fetches instructions** from memory and **executes** them in a sequential order

### Architecture

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/81302f27-4907-4655-bf16-b52b2ac29be7/c0dc4d55-2829-410b-9d69-7a1538c26a6e/Untitled.png)

## CPU components

### CU _control unit_

1. send **control signal** to components of CPU
2. control the **Synchronization of** flow of data around CPU
3. decode instructions - into **operand** and **opcode**
4. controls the **timings** **of operations(Synchronization) - clock speed**
    1. Clock speed is determined by a **system clock**

### ALU (Arithmetic & Logic Unit)

> 1. p**erforms the arithmetic calculations** required to execute the instructions (+,- and shifting)

1. carries out **logical operations**

- It **can be more than one**

-Note: * and / is implemented by series of + - and shifting! -

## Registers

- Register can be **general** or with **specific purpose**

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/81302f27-4907-4655-bf16-b52b2ac29be7/de7fadc1-3087-4e44-a511-4ba4de2f43f9/Untitled.png)

### PC - Program Counter

- stores the _**address**_ of the _**next**_ instruction to **be fetched from memory**
- It will be **incremented** within one cycle of FED
    - **Said to be incremented by 1**
    - _might not be all the case (小声)_

### MAR - Memory Address Register

- stores **the address of the instruction or data** to be _**fetched**_ from or _**written**_ to memory

### MDR - Memory Data Register

1. stores the _**data**_ that has been _**fetched**_ from memory or being _**written**_ to memory
    1. Data from MDR is sent to _**ALU**_ to be processed

### CIR - Current Instruction Register

- stores the _**instruction**_ the CPU is currently _**decoding**_ or _**executing**_

### ACC - Accumulator

- Used when carrying out ALU calculations
- stores the temporary data during the calculations

## System Buses

- _**Buses**_ are used in computers as **parallel transmission components**
    - Each wire can transmit one single bit per unit time

### Control bus

- bidirectional
- usually 8-bit wide

### Data Bus

- Bidirectional
- Larger word length → better the computer performance

### Address Bus

- **unidirectional**
- Address can’t be carried back to CPU
- **Width of buses** determine the amount of address can be accessed

## FDE cycle

- It is the sequence of steps used by the CPU to process each instruction in sequence.

### 1. Fetch

- the address of instruction or data is transferred to the Memory-Address Register from Program Counter. The data/instruction fetched from that address will passed to MDR.
- If it is a instruction, it will be passed to the Current Instruction Register
- The **program counter** then will be incremented by 1

### 2. Decode

- **instruction set** -
    - a collection of all instructions that can be processed and executed by CPU.
    - Each of these instruction has a **unique binary value** that represents it function and a mnemonic such as SUB and ADD that is easier to remember
- the CU use a instruction set to decode the instruction in the instruction set to operands and opcodes

### 3. Execute

- The decoded instruction then can be execute. The arithmetic and logical behaviour can be carried out by the ALU
- some temporary interim result will be stored in the ACC
- The CPU passes the **decoded instruction** as a _**set of control signals**_ to the appropriate components within the computer system

## CPU performance

- 3 key determinants

### Cores

- numbers of cores
    - **more cores** a computer has the more _**instructions**_ that can be executed per second resulting in **better performance (more _FDE cycle_ at the same time)**
    - **doesn’t increase the efficiency directly**, but improved performance when there is large amount of data
- **Drawbacks**
    1. The need for the CPU to communicate with each core will reduce overall performance
        
        ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/81302f27-4907-4655-bf16-b52b2ac29be7/ca9e3f1d-2a38-445c-b4a6-9e05b56cf667/Untitled.png)
        

### Cache size

- used for storing **frequently used instructions/data that need a fast access**
- instructions that are to be fetched and executed next in a process.

### Clock speed

- determine how many instructions the core can **execute each second**
- measured in Hertz
- 1GHz = 1 bili
- To increase performance: Overlocking
    1. Might overheat
    2. Might unsynchornize

## Instruction Set

- _**a collestion of all instructions that can be processed and executed by a CPU. Each instruction is a unique binary code that has a unique mnemonic that indicates its function such as ADD and SUB**_
- After an instruction is decoded into an **opcode and an operand**, the CPU finds the opcode in the processor’s instruction set. It then knows what operation to perform when executing the instruction
- **machine-specific**
- not portable

# Embedded System

### **Properties**

- the computer system with **limited specific built-in functions**
    
- It is used to perform dedicated tasks with a **larger mechanical device**
    
- runs on firmware
    
- doesn’t have additional peripherals
    
- Embedded systems can use either **microprocessors,** **microcontrollers or Soc**
    

### Microcontroller

- Integrated circuit containing a _**CPU**_ and some _**memory**_ (RAM or ROM) built in to the same chip
- designed for specific control or automation tasks
- designed for specific tasks and are thus more efficient
- less powerful but more cost-effective, consume less power

### **Microprocessor**

- Integrated circuit containing only a CPU on the chip
    - RAM , ROM , peripherals need to be added
- capable of executing complex instructions
- used in system that **require high processing power** and **flexibility**

### System on Chips (SoC)

- It contain a _**microcontroller**_ and _**other components**_, such as I/O ports, secondary storages **on a single microchip**

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/81302f27-4907-4655-bf16-b52b2ac29be7/9d409299-5119-4fc0-928d-a4a689ece48f/Untitled.png)

- It shouldn’t be reprogrammed by user
- examples
    - digital clock
    - vending machine
- **advantages**
    - low power consumption than general-purpose computer system
    - small physical size
    - **High Efficiency**
    - **Lower Cost**
    - Good reliability **and Stability**
    - **Simplified User Interface**
    - good **Integration with Other Systems**: