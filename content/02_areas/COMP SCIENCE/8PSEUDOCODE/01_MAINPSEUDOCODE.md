---
draft: false
---
### MAINTAINABLE PROGRAM (need to write well on tests)
#### Meaningful identifier names
#### modules have to be divided and commented appropriately
EX. NO `i` for iterator, use iterator jiterator lmao **NEED TO DECLARE ITERATORS**

[[Bubble Sort]] has lots of examples


maybe you can `OUTPUT array`
just like that

NOT != IT IS **<>**

```
OUTPUT "ask something"
INPUT var
```
to input stuff

`REAL` - float, decimals
`BOOLEAN` - not bool

**Identifiers** cannot start with digits, cannot include other characters (no underscores). only letters and digits.

## **index starts at 1**
##### **no `string[index]`**, use **`SUBSTRING(string, index, 1)` instead**

# [[02_areas/COMP SCIENCE/7/Files|Files]] HERE TO HANDLE FILES NEED
[[02_areas/COMP SCIENCE/7/Bubble Sort|Bubble Sort]]
[[02_areas/COMP SCIENCE/7/Linear Search|Linear Search]]


you have to `DECLARE` everything before using them

`OUTPUT` should not contain any operations
	ex. no `OUTPUT LENGTH(str)`, do `DECLARE len : INTEGER \n len <- LENGTH(str) \n OUPUT len`


#### NOT \==, ITS =

Bubble sort
```
FOR iterator <- 1 TO LENGTH(DataArray) - 1
	FOR jiterator <- 1 TO LENGTH(DataArray) - iterator
		IF DataArray[jiterator] > DataArray[jiterator+1] THEN
			DECLARE temp : REAL
			temp <- DataArray[jiterator]
			DataArray[jiterator] <- DataArray[jiterator+1]
			DataArray[jiterator+1] <- temp
		ENDIF
	NEXT jiterator
NEXT iterator
```
Linear search
```
DECLARE found : BOOLEAN
found <- FALSE
FOR ArrayIndex <- 1 TO 
	IF found = FALSE THEN
		IF DataArray[ArrayIndex] = SearchValue THEN
			found <- TRUE
			OUTPUT "Found at", ArrayIndex
		ENDIF
	ENDIF
NEXT ArrayIndex
```

### IF
NO ELSEIF STATEMENT **ONLY ELSE**
```
IF adfjlasdfj THEN
ELSE
	IF THEN

	ENDIF
ENDIF
```

ex.
```
DECLARE count : INTEGER
count <- 0
FOR i <- 1 TO 10
	FOR j <- 1 TO 5
		count <- count + 2
	NEXT j
NEXT i
OUTPUT count
```

```pseudocode
DECLARE rows : INTEGER
DECLARE display, spaces, stars : STRING

OUTPUT "enter how big the triangle should be"
INPUT rows

FOR i <- 1 TO rows
    spaces <- ""
    stars <- ""

    FOR k <- 1 TO (rows - i)
        spaces <- spaces & " "
    NEXT k

    FOR j <- 1 TO i
        stars <- stars & "*"
    NEXT j
    FOR j <- 1 TO (i - 1)
        stars <- stars & "*"
    NEXT j

    display <- display & spaces & stars & "\n"
NEXT i

OUTPUT display
```
triangle
#### REMEMBER FOR "next" has to contain the iterator so its "NEXT i"


Pseudocode [[02_areas/COMP SCIENCE/8PSEUDOCODE/Library Routines]]
	`ROUND(<identifier>,<places>)`
	`RANDOM()`
	`DIV(<i1>,<i2>)`
	`MOD(<i1>,<i2>)`
	`LENGTH(str)`
	`LCASE(str)`
	`UCASE(str)`
	`SUBSTRING(str,start, length)`
#### SUBSTRING
`SUBSTRING(str,start, length)`
gets the substring from the `start` index to `length`+`start`
`length` + `start` cannot be bigger than the string length.
pseudocode index starts at 1.
```
DECLARE str:STRING
str<-"hello there"
str<-SUBSTRING(str, 5,6)
OUTPUT str

//outputs "o there"
```



#### ROUND
`ROUND(<identifier>,<places>)`
```
real <- ROUND(12.782 , 2)
//real = 12.78

real <- ROUND(12.782,1)
//real = 12.8

real <- ROUND(12.782,0)
//real = 13.0, if integer then 13
```

#### RANDOM
returns a random number between 0 and 1 inclusive.
can be manipulated to different ranges
multiply essentially means the max, and addition means the min
```
value <- RANDOM()


//0.0-6.0
value <- RANDOM()*6

//4.0-10.0
value<-RANDOM()*6+4
```

#### MOD and DIV
```
value <- MOD(5,3)
//value = 2

value <- DIV(5,3)
//value = 1
```
