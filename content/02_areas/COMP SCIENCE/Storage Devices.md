```toc
```

# Primary Memory

## Characteristics

- It can be directly accessed by the CPU
- They are all part of the CPU or motherboard
- It can be volatile or non-volatile

## RAM - Random Access Memory

### Properties

1. **Volatile** - contents are lost when powering off the computer
2. It acts as a **temporary memory** - data can be changed when a computer system is operating
3. It is used to store the part of data, any files, and instructions **currently in use**.
4. It is possible to **increase the amount** of RAM by adding new ones

### DRAM

- It has millions of **transistors** and **capacitors**
    
    - Transistors - holding data (0s and 1s)
    - Capacitors - act as a switch to control the circuit
- It needs to be constantly refreshed (every 15ms)
    
- **Advantages**
    
    1. less expensive to manufacture
    2. consume less power
    3. higher memory capacity
- It is usually used to construct the **main memory**
    

### SRAM

- It doesn’t need to be constantly refreshed
    
- It uses flip-flops to hold memory
    
- It is much faster to access
    
- It is usually used to construct CPU cache
    

## ROM - Read Only Memory

- It is **non-volatile** - content won’t lost after powering off
- It is **permanent memory** - content can’t (hard to) alter and fixed
    - content can only be read
- It stores data and instructions that the computer needs to access when powering up
    - e.g. Firmware, bootloader(bootstrap), BIOS

## Cache

- Three types: L1, L2, L3
- stores the most frequently used data by the CPU

# Secondary Storage

- The type of memory that can not be directly accessed by the CPU
- They are all **non-volatile**
- It stores all data that is _**not required by the CPU currently**_
- They are much **cheaper** than primary storage devices per unit capacity
    - It tends to have a **larger capacity** than the primary memories
- Access time is **slower** than primary memories

## Solid State

- Data is recorded by flashing onto solid chips without moving parts

### SSD - Solid State Drive

**Characteristics**

- It is a **flash memory**
- no moving part (no latency) → more reliable
- It uses **NAND** or **NOR** technologies
- A type of EEPROM**(Electrically Erasable Programmable Read - Only Memory)** technology
- Data is read and written **sequentially**
- It uses **floating gates** and **control gates**
    - It is to control the _**electron movement**_ within chips
    - data is stored as **0s and 1s** in millions of tiny **transistors**

**Floating gate and control gate transistors**

1. SSD contains cells of transistors that are laid out in a grid
2. The intersection of the row and columns of transistors are the cells
3. The control gate is on top of the floating gate

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/81302f27-4907-4655-bf16-b52b2ac29be7/d0470545-b99f-46c0-aa54-7866af64f424/Untitled.png)

**Advantages**

1. **No moving part** → more reliable
2. Comsume **less power**
3. It is **thinner** and lighter
4. It is much **cooler** when operating
5. **Much faster data access**
6. It don’t have to set up to speed

**Disadvantages**

1. **short lifespan**
2. Have **limit on the amount of write operations** per unit period(usually20GB)
3. In terms of design, it is not possible to rewrite a piece of data individually, need to be erased per block first

### Memory stick/SD Card

- It is small, capable to transfer files or be a daongle

## Magnetic

- Mechanical parts move over the disk surface to read and write data magnetically

### HDD - Hard disk drive

- It has a number of **platters** that can spin at about 7000 times a second
- Data is stored on the magnetic surface of the disks(platters) as **magentic dots**
- Its **read-write heads** consist of **electromagnets** that are used to read and write data to platters
- **Read-write heads**
    - can move from the center of the disk to the edge of the disk 50 times a second
    - have a **read-write** arm that consists of an **actuator** to help the head move across
    - It uses **electromagnet**
- **Platters**
    - It can be made of aluminum, glass, or a ceramic material
    - Each platter has **two surfaces** to be used
    - A platter is divided into **sectors and tracks**
        - concentric tracks
- **Sector**
    - A sector on a given track contains a **fixed number of bytes**
    - When storing the file, the required **number of sectors** will be allocated
- **Latency**
    - The amount of time it takes for a **specific block of data** on a data track to rotate around to the read-write head
- Data is **sequentially** read, but they might be stored as fragmented parts
    - in the long run, resulting in lower performance

### Removable HDD - An offline storage device

### Magnetic Tape

## Optical

- Use laser to read or write data

### CD - Compact Disc & DVD - Digital Versatile Disc

- Their surface use thin layer of **metal alloy** or **light-sensitive organic dye** to store data
- They both use **red laser** to create and read **pits and lands (”0s” and ”1s”)**
- In default, They both have a **single spiral track** from the centre to the edge
    - the **outer spiral track** of a disc does **run faster** compared to the **inner spiral track**
- Read
    - red laser is shine onto the surface of the disc, the pits and land reflect different amount of light
- Write
    - Red laser

**Layering**

- **CD -** Typically single-layer, single-sided.
    - **Track pitch - larger**
- **DVD -**Can be single-layer or dual-layer, and single-sided or double-sided.
    - Track pitch - smaller

### Blu-ray disc

- Use blue laser to **read&write data** from the pits and lands on the surface of Blue-ray disc
    - wave length and **Track pitch smaller**

# Virtual Memory

- A type if memory that can be temporarily created as an **extension to the RAM**
    - created with a secondary storage

### Purpose

1. Create **larger memory space** for storeing more data that is supposed in use by the operating system
2. **prevent** computer system from **crashing** when RAM is full

### Page & Paging

- A **fixed-length** **contiguous** block of data utilized in VM systems
- Paging - A function that implement by the **memory management** part of OS that is used to **store and retrieve** data from **virtual memory** and copy it to RAM and also the other way around
    - Data going to be used: VM→RAM
    - Inactive data or the oldest: RAM→VM

### Advantage

1. Program that require memory capacity that is **larger** than physical memory can still be executed
2. **No need to waste** RAM space if data is not being used
3. promote **multitasking** or **multiprogramming**
4. reduce the need to expand RAM space

### Disadvantage

1. Disk thrash → too frquent rw head movement → HDD failure → slow CPU performance
2. Slow down the operation of CPU

# Cloud Storage

- A method of data storage that consists of **storing data in servers** from an **remote location**
    - requires an **internet connection**
    - data is **maintained** and back-up by a third party internet service provider

### The importantness of data redundancy

1. Some data are stored on **more than one server** for **more than one pieces**, allow clients to access data at any time while prevent the **risk** of **losing data accidently**

### Three type of Cloud storage

1. Public cloud
    - Consumer and service provider are from different companies
2. Hybird cloud
    1. Combination of private cloud and public cloud
    2. sensitive data inside private cloud, more public information inside public cloud
3. Private cloud
    - services provided behind a company firewall
    - client and provider are from the **same organization** or the provider is specialized for providing services to that particular client

### Benefits

1. **Portability & Availability**
    - Consumer file stored on the cloud can be accessed at **any time any where** as long as there is internet connection
    - data can be **easily shared**
    - any utilities installed in cloud can be automatically updated
2. **Cost-effectiveness**
    - no need for a consumer to buy ad carry an external storage device
3. **Security**
    - Cloud provide the user with remote backup of data, less risk of data lost
4. **scalability**
    1. The storage capacity can be **extended** and **contracted easily**

### Drawbacks

1. Can **only** access them **with a internet connection**
2. Security issue of a third party
    - risky because the risk of **unauthorized access** and branches
3. Cost issue
    - cost-effective initially, but **expensive overtime** due to higher capacity used and charged per unit period
4. Speed
    - **Slow to upload and download** data through internet connection (slower than secondary device locally)