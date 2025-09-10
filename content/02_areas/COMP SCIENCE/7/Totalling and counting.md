---
draft: false
---
Recall
PDLC
programming development life cycle
Analysis - identify the problem and the requirements needed to solve it. Abstraction
Design - Decompose and design the program into sub-systems.
Coding - make the program and iteratively test
Testing - list out expected results with test cases and fix any errors

## green task
totalling is adding all the numbers up, adding the total of all the numbers, hence its name.
counting is counting one by one, increments of one
```
DECLARE money, totalMoney : REAL
money <- 0.010
totalMoney <- 0.0

DECLARE week:INTEGER
FOR week 1 TO 26
	OUTPUT "\n It is week", week
	OUTPUT "You will get $",money
	totalMoney <- totalMoney + money
	money <- money*2
NEXT week
OUTPUT totalMoney
```


## amber task
```
DECLARE total : REAL
total <- 0.0

OUTPUT "enter stuff to total? y\n"
DECLARE in : CHAR
INPUT in
WHILE in = 'y' DO
	OUTPUT "price?"
	DECLARE p : REAL
	INPUT p

	total <- total + p
	
	OUTPUT "enter stuff to total? y\n"
	DECLARE in : CHAR
	INPUT in
ENDWHILE
OUTPUT "total: ", total
```


## red task
```
DECLARE le1, leq2, gr2, : INTEGER
count <- 0

OUTPUT "enter stuff to count their weight? y\n"
DECLARE in : CHAR
INPUT in
WHILE in = 'y' DO
	OUTPUT "weight?"
	DECLARE w : INTEGER
	INPUT w

	IF w < 1 THEN
		le1 <- le1 + 1
	ELSE
		IF w <= 2 THEN
			leq2 <- leq2 + 1
		ELSE
			gr2 <- gr2 + 1
		ENDIF
	ENDIF
	
	OUTPUT "enter stuff to count their weight? y\n"
	DECLARE in : CHAR
	INPUT in
ENDWHILE
OUTPUT "<1kg: ", le1
OUTPUT "<=2kg: ", leq2,
OUTPUT ">2kg: ", gr2
```



WWW
understood totalling and counting

EBI
know how to draw totalling and counting in flowcharts


# min max average
# green task
```
DECLARE scores : ARRAY[1:30] OF REAL
DECLARE lowest : REAL
lowest <- 101.0
//max score 100


DECLARE i : INTEGER
FOR i<-1 TO 30
	INPUT scores[i]
	IF scores[i]<lowest THEN
		lowest <- scores[i]
	ENDIF
NEXT i

OUTPUT lowest
```

# Amber task
```
DECLARE scores : ARRAY[1:30] OF REAL
DECLARE highest : REAL
highest <- -1


DECLARE i : INTEGER
FOR i<-1 TO 30
	INPUT scores[i]
	IF scores[i]>highest THEN
		highest <- scores[i]
	ENDIF
NEXT i

OUTPUT highest
```

# red task
```
DECLARE scores : ARRAY[1:30] OF REAL
DECLARE avg,total : REAL
total <- 0


DECLARE i : INTEGER
FOR i<-1 TO 30
	INPUT scores[i]
	total <- total + scores[i]
NEXT i
avg <- total/30

OUTPUT avg
```

www: know how to avg, min, max find those
values

EBI: try to use while loop to do it