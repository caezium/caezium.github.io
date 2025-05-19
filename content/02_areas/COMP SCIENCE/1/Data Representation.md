```toc
```

# Number Systems

## Binary

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/81302f27-4907-4655-bf16-b52b2ac29be7/62286464-5f56-4b06-a57c-4015b21d8faf/Untitled.png)

- **The binary number system:** a base-2 number system that only uses 0 and 1 to represent all values

### Why do Computers use binary to represent all forms of data?

- Computer hardware such as RAM and SSD consists of **transistors** and **logic gates**
    - they can only store data in **two states**, 1 and 0

### Binary Shift

- Shift left → multiply the binary number by 2^n
- Shift right → divide the binary number by 2^n

### Overflow

- **Overflow error** is the result of carrying out a calculation that produces a value that exceed the maximum memory capacity allocated by a computer

### Two’s Complement

- Used to represent negative binary numbers
- the left-most bit is used to store the sign of the number

<aside> 💡 **Example** 10010011 (**two’s complement**) 01101100 → 01101101 64+32+8+4+1 = 109 Hence, -109

</aside>

### Applications

- To process or store data in logic gates and transistors
- To store data in registers
- To process data on the computer

## Denary

## Hexadecimal

- A base-16 number system that use 16 different values (0-9 and A-F) to represent each different digit
- **4 binary digits** are equal to each **hexadecimal digit**

### Advantages

- Hexadecimal is very convenient than binary in some cases

1. More Compact Representation→less screen space
2. For developer to debug
3. easily understandable

### Applications

1. Error codes
    1. number that refer to the memory location where error happens can be easily represented by a hexadecimal
    2. help the programmer to distinguish from others and to remember it
2. MAC address
    - Standing for Media Access Control
    - It is the **2nd layer** in the OSI model
    - It uniquely identifies a device on the internet
    - In the form NN-NN-NN(Manufacturer)-DD-DD-DD(device)
3. IPv6 address
    - gives a unique address to each device connected to a network identifying their location
    - It is the **3rd layer** in the OSI model
4. HTML color codes
    - HyperText Mark-up Language
    - e.g. #FFFFFF black

## Conversion between number systems

### Binary to Denary

- Just add up to corresponding value together

### Denary to Binary

- successive subtraction of number with power of 2 until 0 reached
    - e.g. 127
        1. 127 - 128 (x) →0
        2. 127 - 64 = 63 →1
        3. 63-32 = 31 → 1
        4. 31-16=15 → 1
        5. 15-8=7 → 1
        6. 7-4=3 →1
        7. 3-2=1 → 1
        8. 1-1=0 → 1
    - Therefore 127_(10) = 01111111_(2)
- Division Method

### Binary to Hexadecimal

- split the binary number into groups of 4 bits
    - less than 4 just fill 0
- each group can be converted to a hexadecimal digit

### Hexadecimal to Binary

- Reverse process of above

# Text, Sound, and images

## Text

- Text is converted to binary to be processed
- Character set - a collection of all characters and symbols. Each one of them have a unique binary that a computer can identify them.

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/81302f27-4907-4655-bf16-b52b2ac29be7/97ddf9ee-53cc-4fbb-915a-24bdc06f170b/Untitled.png)

### ASCII Code

- American Standard Code for Information Interchange
- use 7-bits

(The extended one use 8-bits and contains some non-english characters)

- **Advantages**
    - use less bits per character
- **Disadvantages**
    - Limited representation - It does not contains full non-Western languages
    - Takes more memory per unit of character

### Unicode

- Represent all languages of the world
- It use 2-4 bytes to represent a character
    - can represent approx. 4 billion characters
- **Advantages**
    - Universal standard that covered wide-range of characters, symbols and emojis
    - Reserve a section of the code for private use to enable local version of character to add their own characters
    - Create unambiguous and uniform encoding where each character is represent by a 16-bits or 32-bits value
- **Disadvantages**
    - It increased the size of a text file if used
    - It is not compatible with the character used ASCII code, if they used interchangeably, there will be encoding error

## Sound

### Sampling

- transforming a **analogue** sound into a **digital** sound file by measuring the **amplitude** of sound wave at **set time intervals**
- Process
    1. **amplitude** of the sound wave is first **determined** at set time intervals
    2. each sample is encoded as series of binary digits

### Sampling Resolution(bit depth)

- The number of bits per sample

![The advantage of using a larger sampling resolution](https://prod-files-secure.s3.us-west-2.amazonaws.com/81302f27-4907-4655-bf16-b52b2ac29be7/fcc2eff6-ad35-4978-a654-f95bb0639f53/Untitled.png)

**The advantage of using a larger sampling resolution**

### Sampling rate

- The number of sound samples taken per second
    - Unit: Hz
- Higher sample rate → less time gaps between samples

## Image

### Bitmap images

- made up of two-dimensional matrix of pixels
- Pixel - the smallest component of an image
- color depth
    - the number of bits used to represent each colour
    - That determines the number of different colors that can be represented
- metadata - data that is used to describe a file
    - e.g. the author information of an image
- Image resolution - the number of pixels in an image

### Vector images

- Formats: in .svg
- You don’t need to understand it in depth

# Data Storage & File Compression

## Units

- Bit → basic unit of all computing memory
- Byte

### Default Memory size System

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/81302f27-4907-4655-bf16-b52b2ac29be7/25297703-31cf-4c46-81da-71f2bf0aa354/Untitled.png)

### IEC Memory Size System

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/81302f27-4907-4655-bf16-b52b2ac29be7/84516acc-5573-4d37-86ee-000282fbd0bb/Untitled.png)

## Calculation of File Size

- bandwidth - the maximum rate of transfer data across a network
    - bits per second

## Data Compression

- reduce the size of a file using compression algorithms

### Goal of Data Compression

- Reduce the need for the maximum rate of transfer of data across a network (bandwidth)
- Reduce the time taken to transfer
- reduce the file size to reduce the cost of using cloud storage
    - ISP charge the cost depends on the amount of data

### Lossless File Compression

- use compression algorithm reduces the file size
    - repeat items are identified and indexed
- no permanent data loss

### Lossy File Compression

- permanently removing data

### Run-Length Encoding (RLE)

## Summary from the book

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/81302f27-4907-4655-bf16-b52b2ac29be7/1633d517-52ae-41ee-afbd-339b4fe57e21/Untitled.png)