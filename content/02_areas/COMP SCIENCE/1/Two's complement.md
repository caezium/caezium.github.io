*negative binary numbers*

**the left-most binary digit will be the sign of the whole number and that value will be negative of what it usually is.**
**this is called two's complement**

ex.
0000 0000
128, 64, 32, 16, 8, 4, 2, 1
will be
**-128**, 64, 32, 16, 8, 4, 2, 1
and this can represent
-128 to 127

# NEED TO USE THIS METHOD FOR MARKS
to convert a number into its negative in binary
you can
1. convert it to binary as a positive number
2. invert each value in the binary number, 1 to a 0, 0 to a 1
3. then just add 1

![[02_areas/COMP SCIENCE/1/attachments/Pasted image 20250314113741.png]]






---

recall
a left logical shift will multiply the entire binary number by 2, a right logical shift will divide it by 2. underflow or overflow can occur

## task 1
10110001
-128+32+16+1=-79 

## task 2
-28
28 = 0001 1100
->
11100011
+1
->
11100100

## task 3
-128 to 127
1000 0000 to 0111 1111


## plenary
-54
54 = 0011 0110
->
1100 1001
+1
->
1100 1010


review learning
www understood how to represent negative numbers
ebi find out why it is called a twos complement

