- An operating system (**OS**) is [[software]] that **manages computer hardware** and **provides a platform for running applications**
- It provides **an interface between the user and the hardware** in a computer system
- It **hides the complexities of the hardware** from the user, for example:
    - A user does not need to know 'where' on secondary storage data is kept, just that it is saved for when they want it again
- An operating systems **main functions** can be divided in to **eight** key areas
#### Managing files
a user can create files using [[application software]], the OS allows creation of directories that can store those files within. It also allows users to move files, delete files, name files, and many more.
#### Provides an user interface
A user interface is **how the user interacts with the operating system**
- Examples of user interfaces include:
    - **Command Line Interface (CLI)**
    - **Graphical User Interface (GUI)**
    - **Menu**
    - **Natural language (NLI)**
[[Command Line Interface and Graphical User Interface]]
*What is a menu interface?*
- A menu interface is **successive menus** presented to a user with a **single option at each stage**
- Often performed with **buttons** or a **keypad**
- Examples include
    - **Chip and pin machines**
    - **Vending machines**
    - **Entertainment streaming services**
*What is a natural language interface?*
- A natural language interface (**NLI**) uses the spoken word to respond to spoken or textual inputs from a user
- Examples include
    - **Virtual assistants** - Amazon Alexa, Google Assistant, Siri
    - **Search engines**
    - **Smart home devices**
#### Handles Interrupts
An interrupt 
a signal sent to the processor to tell it something needs its attention
- Interrupt events **require the immediate attention** of the **central processing unit**
- In order to maintain the smooth running of the system, interrupts need to be **handled** and processed **in a timely manner**
- For example, if a user clicks cancel on a file conversion process, a signal is sent from the mouse, **interrupts the processor**, and the operating system will trigger the cancellation routine

is a signal sent from a device or from [[software]] to the microprocessor. This will cause the microprocessor to temporarily stop what it is doing so that it can service the interrupt. 
Interrupts can be caused by
- hardware fault
- input/output process, ex. requires more inputs to continue
- [[software]] errors
- two processes attempting to access the same memory locations 
- data input, ex. key pressed or mouse click
Interrupts allow computers to carry out many tasks or to have several windows open at the same time. 
#### Managing peripherals and devices
a computer cannot be used without **input and output devices, peripherals**. A *driver is a [[software]] that the **translates data*** from the computer to the peripheral and vice versa.
- The OS **allocates system resources** to peripherals to ensure **efficient operation**
- Peripheral management makes **plug-and-play** (PnP) functionality possible, **automatically detecting and configuring new peripherals** without the need for manually installing device drivers or power cycling the system
 
*What is a device driver?*
- A device driver is **a piece of software used to control a piece of hardware**
- Peripherals **require device drivers** in order to be used by the operating system   
- The OS has **generic device drivers built in** which makes **basic compatibility** possible and enables **plug-and-play** (PnP)
- In order for hardware to be used to its **maximum capacity**, often **a separate device driver must be downloaded** from the manufacturer
- Device drivers are **OS specific** and are **regularly updated**
#### Managing user accounts
this can include preferences, keep data separate for multiple accounts, and restricting access.
#### Providing System Security
- Operating systems provide various security features such as password-protected system accounts, a **firewall**, virus scanning and **file encryption**
- Password-protected system accounts are a very common feature in operating systems   
- System accounts can also be restricted from performing certain actions, e.g. editing network settings, installing unapproved [[software]], changing the account settings of other users
#### Multi tasking and Memory management
A single processor can only ever execute one instruction at a time. The processor does this so fast that it appears to be doing several tasks at once. The OS allows this to happen by deciding which processes should be executed next and how long they can spend being processed before switching to another process, using interrupts.
- Memory management is a process carried out by the operating system **allocating main memory (RAM) between different programs** that are **open at the same time**
- The OS is responsible for **copying programs and data from secondary to primary storage** as it is needed
- **Programs and data require different amounts of RAM** to operate efficiently and the OS manages this process
- **RAM is allocated** based on **priority and fairness**, for example, system applications (essential) may have a higher priority than user applications
- The OS **dynamically manages the memory**, adjusting allocation as needed to maintain optimal system performance
- Memory management makes **multitasking** possible
#### Provide a platform for applications to run
- Operating systems provide a **platform** on which **[[application software]] can run**, this is mainly by allowing [[software]] **access to system resources**
- For example, if a computer game has intensive graphics and online play, the operating system will grant it access to the GPU and the network card

![[Operating Systems and Interrupts-20250216204832099.png]]

Operating Systems
provides an interface, manages files, manages peripherals and drivers, manages memory, manages multitasking, manages interrupts, provides a platform for running applications, manages user accounts

[[system software]]
an operating system allows the computer system to function correctly and allow users to communicate with the computer system. Applications can run and interaction between humans and computers.

interfaces GUI and CLI
WIMP: windows, icons, menus, and pointers



Firmware. when a computer starts up, part of the operating system needs to be loaded into RAM, this is known as booting up the computer.
The start-up of the computer's motherboard is handled by the basic input/output system, BIOS. The BIOS tells the computer where the storage device that holds the operating system can be found, then it loads the part of the operating system that is needed and executes it. The BIOS is an example of a firmware.
Firmware is defined as a program that provides low level control for devices.




Buffers are memory areas that stores data temporarily.

Recall
CLI stands for command line interface, it requires users to enter specific instructions using only the keyboard, the entry level for using this interface is quite high, its benefits are that it takes less resources than GUIs and are better for certain situations.
GUI stands for graphical user interface, the user can click on or operate using graphics , it is very easy to use.

# task 1
An operating system is [[software]] that manages the hardware and [[software]] resources of a computer system. It handles peripheral devices, files, and provides an interface.

# task 2
An interrupt is a signal that tells the microprocessor to temporarily stop what it is doing. This allows computers to carry out many task or to have several windows.
Interrupts can be caused by
- two processes attempting to access the same memory locations
- programs requesting for input
- output required for the [[software]] to continue
- error from the hardware

# task 3
A buffer is a memory storing area that stores data temporarily to have data to be passed in and out quickly to allow multiple processes to be serviced.



# plenary
Firmware is a program that provides low level control for devices.
Firmware is often used to start up a device.
The BIOS, basic input/output system, is an example of firmware.
Some examples of [[system software]] are operating systems and  device drivers


Review learning
www
	understood the importance of operating systems and how they use interrupts
ebi
	learn more about firmware