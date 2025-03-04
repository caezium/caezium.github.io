---
draft: false
---
Library routines are pre-defined subroutines that allow you to implement functionality without needing to write your own code.


Pseudocode library routines
	`ROUND(<identifier>,<places>)`
	`RANDOM()`
	`DIV(<i1>,<i2>)`
	`MOD(<i1>,<i2>)`
	`LENGTH(str)`
	`LCASE(str)`
	`UCASE(str)`
	`SUBSTRING(str,start, length)`
## task 1
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

## Task 2
generate a integer between 5-25 inclusive.
```
DECLARE num : INTEGER
DECLARE what : REAL
what <- RANDOM()*25+5
num <- ROUND(what,0)

OUTPUT num
```

## Task 3
```
DECLARE phrase,name : STRING
OUTPUT "name?"
INPUT name

phrase <- "The quick brown fox jumps over the lazy dog"

DECLARE sum : INTEGER
FOR i <- 1 TO LENGTH(name)
	DECLARE flag : BOOLEAN
	flag <- TRUE
	DECLARE j : INTEGER
	j <- 0
	WHILE FLAG DO
		j<-j+1
		IF name[i] == phrase[j] THEN
			sum <- sum + j
			flag <- FALSE
		ENDIF
	ENDWHILE
NEXT i


OUTPUT sum
```
