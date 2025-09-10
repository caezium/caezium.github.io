---
draft: false
---
sorting : sorting content into orders

bubble sort: takes first 2 values then compares theme. if they are wrong way around, swap them. then it takes the second and third values. it repeats until it goes all the way through the list. then after it has worked all the way through the list once, it repeats from the first and second again.
it is called bubble sort because it acts like a bubble moving across all the elements to the end then starting again.


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

recall
linear search is when you search through everything one by one and get an element from a list of data.


# task 1
first pass 34,28,65,52,21,68
second pass 28,34,52,21,65,68
third pass 28,34,21,52,65,68
fourth pass 28,21,34,52,65,68

# task 2
you need 5 passes to sort the list in task 1.
the last number will always be correct after the first pass


# task 3
4 times
```
FOR iterator <- 1 TO 3
	FOR jiterator <- 1 TO 4 - iterator
		IF DataArray[jiterator] > DataArray[jiterator+1] THEN
			DECLARE temp : REAL
			temp <- DataArray[jiterator]
			DataArray[jiterator] <- DataArray[jiterator+1]
			DataArray[jiterator+1] <- temp
		ENDIF
	NEXT jiterator
NEXT iterator
```


Review learning
WWW: understood bubble sort
EBI: how to draw it in flowchart



## plenary
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



# task 4
```
DECLARE names : ARRAY[1:5] OF STRING
DECLARE iterator, jiterator : INTEGER
DECLARE temp : STRING



DECLARE longest : INTEGER
longest<-0
FOR iterator <- 1 TO 5
	OUTPUT "enter name"
	INPUT names[iterator]
    IF LENGTH(names[iterator]) > longest THEN
        longest <- LENGTH(names[iterator])
    ENDIF
NEXT iterator


//cases where some strings are shorter
FOR iterator <-1 TO 5
    IF LENGTH(names[iterator]) < longest THEN
        FOR jiterator <- 1 TO longest-LENGTH(names[iterator])
            names[iterator]<- names[iterator]+"/"
        NEXT jiterator
    ENDIF
NEXT iterator
  
//65-90, slash '/' is 0
FUNCTION ASCII(string : STRING) RETURNS INTEGER
	DECLARE ascii : INTEGER
	ascii <- 0
	DECLARE s : STRING
	s <- UCASE(string)
	DECLARE letters : ARRAY[1:26] OF CHAR
	letters[1] <- "A"
	letters[2] <- "B"
	letters[3] <- "C"
	letters[4] <- "D"
	letters[5] <- "E"
	letters[6] <- "F"
	letters[7] <- "G"
	letters[8] <- "H"
	letters[9] <- "I"
	letters[10] <- "J"
	letters[11] <- "K"
	letters[12] <- "L"
	letters[13] <- "M"
	letters[14] <- "N"
	letters[15] <- "O"
	letters[16] <- "P"
	letters[17] <- "Q"
	letters[18] <- "R"
	letters[19] <- "S"
	letters[20] <- "T"
	letters[21] <- "U"
	letters[22] <- "V"
	letters[23] <- "W"
	letters[24] <- "X"
	letters[25] <- "Y"
	letters[26] <- "Z"
    
	
	
	FOR iterator<-1 TO LENGTH(s)
		DECLARE flag : BOOLEAN
		flag <- TRUE  
		
		DECLARE asci : INTEGER
		asci <- 0
		
		FOR jiterator<-1 TO 26
			IF flag THEN
				IF SUBSTRING(s,iterator,1) = letters[jiterator] THEN
                    asci <- 64+jiterator
                    flag <- FALSE
				ENDIF
			ENDIF
		NEXT jiterator
        ascii <- ascii*100 + asci
		  

	NEXT iterator
	RETURN ascii

ENDFUNCTION


DECLARE i,j : INTEGER
FOR i <- 1 TO 4
	FOR j <- 1 TO 5 - i
		IF ASCII(names[j]) > ASCII(names[j+1]) THEN
			temp <- names[j]
			names[j] <- names[j+1]
			names[j+1] <- temp
		ENDIF
	NEXT j
NEXT i  

FOR i <- 1 TO 5
	OUTPUT names[i]
NEXT i
```



# task 5

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

# task 6
```
DECLARE name : STRING
DECLARE iterator, jiterator : INTEGER
DECLARE temp : STRING
name <- "computersciencelearning"

DECLARE namea : ARRAY[1:23] OF CHAR
FOR iterator <- 1 TO 23
	namea[iterator] <- SUBSTRING(name, iterator, 1)
NEXT iterator

//65-90
FUNCTION ASCII(string : STRING) RETURNS INTEGER
	DECLARE ascii : INTEGER
	ascii <- 0
	DECLARE s : STRING
	s <- UCASE(string)
	DECLARE letters : ARRAY[1:26] OF STRING
	letters[1] <- "A"
	letters[2] <- "B"
	letters[3] <- "C"
	letters[4] <- "D"
	letters[5] <- "E"
	letters[6] <- "F"
	letters[7] <- "G"
	letters[8] <- "H"
	letters[9] <- "I"
	letters[10] <- "J"
	letters[11] <- "K"
	letters[12] <- "L"
	letters[13] <- "M"
	letters[14] <- "N"
	letters[15] <- "O"
	letters[16] <- "P"
	letters[17] <- "Q"
	letters[18] <- "R"
	letters[19] <- "S"
	letters[20] <- "T"
	letters[21] <- "U"
	letters[22] <- "V"
	letters[23] <- "W"
	letters[24] <- "X"
	letters[25] <- "Y"
	letters[26] <- "Z"
	

    DECLARE asci : INTEGER
    FOR jiterator<-1 TO 26
        IF s = letters[jiterator] THEN
            ascii <- 64+jiterator
        ENDIF
    NEXT jiterator
	RETURN ascii
ENDFUNCTION


DECLARE i,j : INTEGER
FOR i <- 1 TO 22
	FOR j <- 1 TO 23 - i
		IF ASCII(namea[j]) < ASCII(namea[j+1]) THEN
			DECLARE temp : STRING
			temp <- namea[j]
			namea[j] <- namea[j+1]
			namea[j+1] <- temp
		ENDIF
	NEXT j
NEXT i


name <- ""
FOR iterator <- 1 TO 23
	name<-name+namea[iterator]
NEXT iterator
OUTPUT name
```

Review learning
WWW: know how to bubble sort and convert to ascii manually in pseudocode
EBI: optimize the code


![[Bubble Sort-20241120222057210.png]]