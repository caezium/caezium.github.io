
Computers only process binary, so all data must be converted to binary to be processed by a computer.
So text also has to be converted to binary/numbers.

**To convert text to binary, it uses a tool called a character set. The two main character sets that a computer can use is ASCII and UNICODE.**

a character set is **a set of letters, symbols, and digits that can be represented by a computer.**

**Text is converted using character sets by looking up the corresponding character code for that character in the character set. Each character has a unique code in the set.**

## ASCII
American standard code for information interchange
7 bits -> 127 possible characters

Extended ASCII later developed, 8 bit -> 255 possible characters


![[02_areas/COMP SCIENCE/1/attachments/Pasted image 20250318101449.png]]

![[02_areas/COMP SCIENCE/1/attachments/Pasted image 20250318101519.png]]


## Unicode
Universal character encoding

different bit sizes
8 bit, 16 bit, 24 bit, 32 bit
16 bit can represent around 65 000 characters, 32 can represent 2,147,483,647 characters




---

recall
computers can only read binary number as on and off signals. hexadecimal is used by humans to represent binary numbers because it is easier to read by a digit factor of 4. we can use the two's complement to represent negative numbers, where the most left digit of a binary number is used to represent a negative version of what itself is usually is.
## task 1
ASCII uses 7 bits, which can only represent 127 different characters/combinations. Unicode has several different version, like 32 bit, which can represent around 2 billion possible characters. ASCII was used to display American/english alphabet and symbols, but when other languages require more than 127 Unicode, people developed Unicode to be able to take all that stuff, even emojis.

ASCII hexadecimal representation of the URL www. facebook.com
%77 %77 %77 %2E %66 %61 %63 %65 %62 %6F %6F %6B %2E %63 %6F %6D


## task 2
there are several different character sets available.
eg. ASCII, extended ASCII, Unicode 8 bit, Unicode 16 bit, Unicode 24 bit, Unicode 32 bit. (UTF-8, UTF-16, UTF-32)

Unicode was adapted as the international standard for character coding because it can store way more characters than ASCII as it uses more bits, this allows several different languages with a lot of characters, such as Chinese, to be able to be represented.

## task 3
question 1

```py
age = input("Enter your age in years (between 0-8):")

charNum = ord(age)
charNum += 1

age = chr(charNum)
print(age)
```

(a)
ord() returns the Unicode of the character passed through it, so ord(age) is getting the Unicode representation of what the user just inputted.

(b)
line for adds 1 to the Unicode decimal representation of the age variable

(c) ord only works on single characters, chr also only takes one single character. the program can break it it gets to double digits converted to unicode or added one to it to be double digits.

![[Excalidraw/Drawing 2025-03-18 10.39.22.excalidraw]]

question 2

```py
firstNum = input("Enter first number:"))
secondNum = input("Enter second number:"))

print(firstNum + secondNum)
sum = int(firstNum) + int(secondNum)
print(sum)
```
input 3 and 17, outputs: 317 \n 20
![[Excalidraw/Drawing 2025-03-18 10.49.07.excalidraw]]


## Plenary
worksheet


```py
n = 0x0001F602

for i in range(100):
	print(chr(n+i))
```

review learning
www understood where character sets originated from and why they were designed/improved on
ebi remember acronyms and how to represent some characters for these character sets