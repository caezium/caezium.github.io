---
draft: false
---
Linear search is searching for an item by checking one by one in a list. **Sequentially**

RECALL
totalling- total of numbers
counting- counting with increments of one

## Task 1
Linear search examines items one by one in a list and  checks them one by one to see if the item has been found. This search is very easy to make but very slow because its time complexity is O(n), meaning that in the worst case scenario, the item is on the end of the list and you would have to loop through the whole list to find it.

## Task 2
Searched may have to be carried out when finding an item in a shopping app or finding a student's profile in the school system.

## Task 3
```
DECLARE names : ARRAY[1:5] OF STRING
names[1] <- "MR MAC"
names[2] <- "MISS HANNAH"
names[3] <- "MR BARTON"
names[4] <- "MISS SHEVANI"
names[5] <- "MISS SHAHLA"


FUNCTION LinearSearch(q:STRING) RETURNS INTEGER
	DECLARE index : INTEGER
	FOR index <- 1 TO 5
		IF names[index] = q THEN
			RETURN index
		ENDIF
	NEXT index
	RETURN -1
ENDFUNCTION

DECLARE query : STRING
INPUT query
query <- UCASE(query)

DECLARE where : INTEGER
where <- LinearSearch(query)
IF where = -1 THEN
	OUTPUT "NOT FOUND"
ELSE
	OUTPUT where
ENDIF
```


Review learning
WWW
	know how linear search works
EBI
	draw linear search in flowcharts




## Task 4
```
DECLARE found : BOOLEAN
found <- FALSE
DECLARE index : INTEGER
index <- 0
WHILE found = FALSE DO
	index <- index + 1
	IF resort[index] = townName THEN
		found <- TRUE
	ENDIF
ENDWHILE
OUTPUT index
```

## Task 5
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

## Task 6
```
FUNCTION LinearSearch(q:STRING) RETURNS INTEGER
	DECLARE index : INTEGER
	FOR index <- 1 TO 7
		IF ids[index] = q THEN
			RETURN index
		ENDIF
	NEXT index
	RETURN -1
ENDFUNCTION

DECLARE query : INTEGER
OUTPUT "which id would you like to search for"
INPUT query

DECLARE foundAt : INTEGER
foundAt <- LinearSearch(query)
OUTPUT foundAt
```

Review learning
WWW
	know how linear search works
EBI
	draw linear search in flowcharts