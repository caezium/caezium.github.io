---
draft: false
---
**Index** starts at **1**
`LENGTH()` - returns length of str, including spaces
`LCASE()` - lower case string
`UCASE()` - upper case string
`SUBSTRING(str, startINTEGER, endINTGER` - substring select

## Task 1
	create a Python program to calculate the number of vowels in a string.
```pseudocode
DECLARE text : STRING
OUTPUT "enter something"
INPUT text
text <- UCASE(text)

DECLARE vowels : INTEGER
vowels <- 0
//presuming vowels are all AEIOUs.
FOR i<-1 TO LENGTH(text)
	IF text[i] == 'A' OR text[i] == 'E' OR text[i] == 'I' OR text[i] == 'O' OR text[i] == 'U' THEN
		vowels <- vowels+1
	ENDIF
NEXT

OUTPUT vowels
```
```py
text = input("enter something)
text = text.upper()
vowels = 0
for i in range (0,len(text)):
	if text[i] in ('A','E','I','O','U'):
		vowels += 1
print(vowels)
```
## Task 2
	write a pseudocode algorithm which allows the user to enter a name consisting of a first name and a surname, and outputs the name in uppercase letters and the length of the name

```pseudocode
DECLARE first : STRING
DECLARE last : STRING

OUTPUT "enter your first name pls:"
INPUT first
OUTPUT "enter your last/surname pls:"
INPUT last

DECLARE len : INTEGER
len <- LENGTH(first+last)

DECLARE upper : STRING
upper <- UCASE(first+last)

OUTPUT upper,len

```

## Task 3
	write a pseudocode algorithm which allows a user to enter a product code, ex. AFG191214726, and outputs character4-6 and the last character of the code.
```pseudocode
DECLARE code : STRING
OUTPUT "product code?"
INPUT code

DECLARE middle : STRING
middle <- SUBSTRING(code, 4,6)

DECLARE last : CHAR
last <- code[LENGTH(code)]

OUTPUT middle
OUTPUT last
```

