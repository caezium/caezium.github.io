---
draft: false
---
# 2D Arrays
table with rows and columns
`DECLARE what : ARRAY[1:3,1:5] OF INTEGER`
3 rows, 5 columns
`what[1,3] <- what[row, column]`
element of row 1, column 3
**NUMBER OF ROWS : NUMBER OF COLUMNS**


### Extended writing
Video games shouldn't be in the olympics because there are too many of them, until one game massively dominates the gaming industry, then no.
## Task 1
1d arrays are like a list, 2d arrays are like tables.

## Task 2
```
DECLARE Elements : ARRAY[1:3,1:5] OF STRING

Elements[1,3] <- "Antimony"
Elements[1,2] <- "Sb"
Elements[1,3] <- "Stibium"

Elements[2,1] <- "Copper"
Elements[2,2] <- "Cu"
Elements[2,3] <- "Cuprum"

Elements[3,1] <- "Gold"
Elements[3,2] <- "Au"
Elements[3,3] <- "Aurum"

Elements[4,1] <- "Iron"
Elements[4,2] <- "Fe"
Elements[4,3] <- "Ferrum"

Elements[5,1] <- "Lead"
Elements[5,2] <- "Pb"
Elements[5,3] <- "Plumbum"
```

## Task 3
```
DECLARE ClassScores : ARRAY[1:20,1:5] OF STRING

DECLARE iterator, jiterator : INTEGER
FOR iterator <- 1 TO 5
	FOR jiterator <- 1 TO 20
		OUTPUT "student no.",jiterator," subject", iterator, "score:"
		INPUT ClassScores[iterator,jiterator]
	NEXT jiterator
NEXT iterator
```


### Review learning
WWW: understood how to declare 2d arrays in pseudocode
EBI: stop getting confused with first index and second index/ when rows when columns

## Plenary
```
DECLARE numbers : ARRAY[1:10,1:20] OF INTEGER

DECLARE iterator,jiterator : INTEGER
FOR iterator <- 1 TO 10 
	FOR jiterator <- 1 TO 20
		numbers[iterator,jiterator] <- RANDOM()*100+1
	NEXT jiterator
NEXT iterator
```



---
processing 2d arrays


## Task 1
```
OUTPUT "how much info/data needs to be stored for each element?"
DECLARE size : INTEGER
INPUT size

DECLARE Elements : ARRAY[1:118,1:size] OF STRING
//______|element name|
// stuff|------------|

DECLARE iterator, jiterator : INTEGER
FOR iterator <- 1 TO 118
	OUTPUT "element", iterator
	FOR jiterator <- 1 TO size
		OUTPUT "data no.",jiterator
		INPUT Elements[jiterator,iterator]
	NEXT jiterator
NEXT iterator

```

## Task 2 and 3
```
DECLARE ClassScores : ARRAY[1:20,1:5] OF INTEGER
//________|Students|
//Subjects|--------|

DECLARE iterator, jiterator : INTEGER
FOR iterator <- 1 TO 5
	FOR jiterator <- 1 TO 20
		OUTPUT "student no.",jiterator," subject", iterator, "score:"
		INPUT ClassScores[iterator,jiterator]
	NEXT jiterator
NEXT iterator


//display
FOR iterator <- 1 TO 5
	FOR jiterator <- 1 TO 10
		OUTPUT "student",jiterator,"subject",iterator,"score:",ClassScores[iterator,jiterator]
	NEXT jiterator
NEXT iterator

//calculate sum
DECLARE sum : INTEGER
FOR iterator <- 1 TO 5
	FOR jiterator <- 1 TO 20
		sum <- sum + ClassScores[iterator,jiterator]
	NEXT jiterator
NEXT iterator
OUTPUT sum
```

### Review learning
WWW: understood how to process data and stuff using 2d arrays
EBI: try to write 2d arrays stuff faster



## Plenary
```
DECLARE MyData : ARRAY[1:20,1:5] OF STRING
//_____|1|...20|
//    1|-|-----|
//  ..5|-|-----|

DECLARE searchRow,searchColumn : INTEGER
OUTPUT "search row"
INPUT searchRow
OUTPUT "searchColumn"
INTPUT searchColumn

DECLARE flag : BOOLEAN
flag <- TRUE
IF searchRow > 5 THEN
	flag <- FALSE
ENDIF
IF searchColumn > 20 THEN
	flag <- FALSE
ENDIF
OUTPUT flag
```