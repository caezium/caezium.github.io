#### What is a logical binary shift?
- A logical binary shift is how a computer system performs **basic multiplication and division** on non-negative values (0 and positive numbers)
- Binary digits are **moved left** or **right** a set number of times
- A left shift **multiplies** a binary number by 2 (x2
- A right shift **divides** a binary number by 2 (/2)
- A shift can move more than one place at a time, the principle remains the same
- A left shift of 2 places would multiply the original binary number by 4 (x4)

#### How do you perform a logical left shift of 1?
- Here is the binary representation of the denary number 40

|**128**|**64**|**32**|**16**|**8**|**4**|**2**|**1**|
|---|---|---|---|---|---|---|---|
|**0**|**0**|**1**|**0**|**1**|**0**|**0**|**0**|

- To perform a left logical binary shift of 1, we move each bit 1 place to the left
- The digit in the 128 column (**MSB**) will move left causing an **overflow error**
- The 1 column becomes empty so is filled with a 0

| **128** | **64** | **32** | **16** | **8** | **4** | **2** | **1** |          |
| ------- | ------ | ------ | ------ | ----- | ----- | ----- | ----- | -------- |
|         | **0**  | **1**  | **0**  | **1** | **0** | **0** | **0** | **= 40** |
| **0**   | **1**  | **0**  | **1**  | **0** | **0** | **0** | **0** | **= 80** |

- The original binary representation of denary **40** (32+8)  was **multiplied by 2** and became **80** (64+16)
    

#### How do you perform a logical left shift of 2?

- Here is the binary representation of the denary number 28

|**128**|**64**|**32**|**16**|**8**|**4**|**2**|**1**|
|---|---|---|---|---|---|---|---|
|**0**|**0**|**0**|**1**|**1**|**1**|**0**|**0**|

- To perform a left binary shift of 2, we move each bit 2 places to the left
- The digit in the 128 (**MSB**) and 64 column will move left causing an **overflow error**
- The 1 and 2 column become empty so are filled with a 0
    

| **128** | **64** | **32** | **16** | **8** | **4** | **2** | **1** |           |
| ------- | ------ | ------ | ------ | ----- | ----- | ----- | ----- | --------- |
|         |        | **0**  | **1**  | **1** | **1** | **0** | **0** | **= 28**  |
| **0**   | **1**  | **1**  | **1**  | **0** | **0** | **0** | **0** | **= 112** |

- The original binary representation of denary **28** (16+8+4)  was **multiplied by 4** and became **112** (64+32+16)
    
#### How do you perform a logical right shift of 1?
- Here is the binary representation of the denary number 40

|**128**|**64**|**32**|**16**|**8**|**4**|**2**|**1**|
|---|---|---|---|---|---|---|---|
|**0**|**0**|**1**|**0**|**1**|**0**|**0**|**0**|

- To perform a right binary shift of 1, we move each bit 1 place to the right    
- The digit in the 1 column (**LSB**) will  move right causing an **underflow error**
- The 128 column becomes empty so is filled with a 0
    

| **128** | **64** | **32** | **16** | **8** | **4** | **2** | **1** |          |
| ------- | ------ | ------ | ------ | ----- | ----- | ----- | ----- | -------- |
| **0**   | **0**  | **1**  | **0**  | **1** | **0** | **0** |       | **= 40** |
| **0**   | **0**  | **0**  | **1**  | **0** | **1** | **0** | **0** | **= 20** |

- The original binary representation of denary **40** (32+8)  was **divided by 2** and became **20** (16+4)
#### How do you perform a logical right shift of 2?
- Here is the binary representation of the denary number 200

| **128** | **64** | **32** | **16** | **8** | **4** | **2** | **1** |
| ------- | ------ | ------ | ------ | ----- | ----- | ----- | ----- |
| **1**   | **1**  | **0**  | **0**  | **1** | **0** | **0** | **0** |

- To perform a right binary shift of 2, we move each bit 2 places to the right    
- The digits in the 1 (**LSB**) and 2 columns will move right causing an underflow error
- The 128 and 64 columns become empty so are filled with a 0

| **128** | **64** | **32** | **16** | **8** | **4** | **2** | **1** |           |
| ------- | ------ | ------ | ------ | ----- | ----- | ----- | ----- | --------- |
| **1**   | **1**  | **0**  | **0**  | **1** | **0** |       |       | **= 200** |
| **0**   | **0**  | **1**  | **1**  | **0** | **0** | **1** | **0** | **= 50**  |

- The original binary representation of denary **200** (128+64+8) was **divided by 4** and became **50** (32+16+2)






---

Recall
Binary is a base-two number system, that can be read by a computer
Hexadecimal is a base-16 number system, it is easier to read for a human


## tasks
1
a
97h =1001 0111
6Ch =0101 1100

b
Hexadecimal can also be used to represent color for websites and markup languages like HTML.
It can also be used in Internet Protocol Addresses.

c
i) 01001000
ii)Because it shifted by 2, the number is multiplied by 2 to the power of 2 which is 4.


2
167 = 1010 0111
214 = 1101 0110

3
028h =0000 0010 1000 =40
1A9h =0001 1010 1001 =9+160+256=425 
20Ch =0010 0000 1100 =512+12=524 


4
43h =0100 0011
B7h =1011 0111
F0h =1111 0000

5a
1. correct
2. incorrect
3. incorrect
4. incorrect

5b
1100 0100 0000 =64 + 1024 + 2048= 3136

## Plenary
a
i) 
A = 65 = 0100 0001
C=12 = 0000 1100
ii) 
65 = 41h
12 = 0Ch

b
1111 1010 1001 0111 = 
FA97h





Review learning
WWW: converted them not so slow
EBI: faster and more accurate, remember multiples of 16 for faster binary and hexadecimal to denary