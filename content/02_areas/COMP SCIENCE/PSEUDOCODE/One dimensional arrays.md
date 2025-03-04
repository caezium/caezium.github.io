---
draft: false
---
## Recall
*"It is unreasonable to expect privacy in the age of social media and the internet"*
Yes, I think it is very unreasonable to expect privacy because you are essentially sharing your private life/information online. Even with the highest amount of protection, there are still ways for your data to breach and get exposed. 


**Arrays Pseudocode**
index starts at 1
`DECLARE name : ARRAY[1:20] OF STRING`
`name[1] <- "what"`
`OUTPUT name[1]` outputs 'what'

```
FOR iterator <- 1 TO 20
	OUTPUT name[iterator]
NEXT iterator
```

## Task 1
1. the difference between a variable and array is that an array can store lists of data and a variable can only store one.
2. the algorithm will result in an error because they are assigning a different data type that is to the array.

## Task 2
```
DECLARE nums : ARRAY[1:10] OF REAL
OUTPUT "10 nums pls"

//iterating through inputs to store the 10 numbers users inputted into a 1d array
FOR iterator <- 1 TO 10
	INPUT nums[iterator]
NEXT iterator
```

## Task 3
```
DECLARE StudentMarks : ARRAY[1:100] OF REAL
OUTPUT "enter the students grades"

//adding together the 100 inputted student marks
DECLARE sum, average : REAL
sum <- 0.0
FOR iterator <- 1 TO 100
	INPUT StudentMarks[iterator]
	sum <- sum + StudentMarks[iterator]
NEXT iterator

OUTPUT "sum: ", sum
avg <- sum/100
OUTPUT "avg: ", avg
```


### Review learning
WWW: i understood how to write and use an array in pseudocode
EBI: remember that no space after `ARRAY[1:<len>]`'s ARRAY.


## Plenary
Array: a data structure that store a collection of elements.
Array dimension: number of indices needed to access an element in the array, ex. a 2D array is a table, 3D can represent a cube.
Array index: the position of each element in an array is their index. the elements can be accessed through the use of their index.


# **Practice**
parallel arrays - more than one array that are storing related data are called parallel arrays. item names and price

## recall
arrays are written like this is pseudocode `DECLARE name : ARRAY[start:end] OF STRING`
indexes start at 1

## Task 1
```
DECLARE MyNumbers : ARRAY[1:10] OF INTEGER

//square of nums in MyNumbers
DECLARE Squares : ARRAY[1:10] OF INTEGER

//initializing values and squaring them
FOR iterator <- 1 TO 10
	MyNumbers[iterator] <- iterator
	Squares[iterator] <- iterator*iterator
NEXT iterator
```

## Task 2
```
DECLARE nums : ARRAY[1:10] OF INTEGER

OUTPUT "input 10 integers pls"
//input 10 nums
FOR iterator <- 1 TO 10
	INPUT num[iterator]
NEXT iterator

//how many odds and evens
DECLARE Evens, Odds : INTEGER
FOR iterator <- 1 TO 10
	IF num[iterator]%2 == 0 THEN
		evens <- evens + 1
	ELSE
		odds <- odds +1
	ENDIF
NEXT iterator
OUTPUT "evens:", evens, "\nodss:", odds
```

## Task 3
```
DECLARE Ages : ARRAY[1:25] OF INTEGER
OUTPUT "input the students ages pls"
//input ages
FOR iterator <- 1 TO 25
	INPUT Ages[iterator]
NEXT iterator

DECLARE MaxAge, MinAge, Sum : INTEGER
DECLARE Avg : REAL
MaxAge <- Ages[1]
MinAge <- Ages[1]
//average of ages rounded to 1 dp
//highest and lowest
FOR iterator <- 1 TO 25
	DECLARE current : INTEGER
	current <- Ages[iterator]
	Sum <- Sum + current
	IF current < MinAge
		MinAge <- current
	ENDIF
	IF current > MaxAge
		MaxAge <- current
	ENDIF
NEXT iterator
Avg <- sum/25
Avg <- ROUND(Avg, 1)

OUTPUT "lowest age: ", MinAge
OUTPUT "highest age: ", MaxAge
OUTPUT "average age: ", Avg
```

### Review learning
WWW: declared arrays and used them to achieve the task
EBI: remember how to declare arrays

## Extended Task
```
DECLARE StudentNames : ARRAY[1:15] OF STRING
DECLARE ArrMaths, ArrPhysics : ARRAY[1:15] OF REAL

//we are assigning a random number for student grades because the teacher is too lazy to mark their work
PROCEDURE populateArrays
	OUTPUT "student names"
	FOR iterator <- 1 TO 15
		INPUT StudentNames[iterator]
		ArrMaths[iterator] <- RANDOM()*100
		ArrPhysics[iterator] <- RANDOM()*100
	NEXT iterator
ENDPROCEDURE

PROCEDURE StudentAvg
	DECLARE sum, avg : REAL

	FOR iterator <- 1 TO 15
		OUTPUT StudentNames[iterator]," Maths: ", ArrMaths[iterator], " Physics: ", ArrPhysics[iterator]
		sum <- sum + ArrMaths[iterator] + ArrPhysics[iterator]
	NEXT iterator
	avg <- sum/30
	OUTPUT "avg: ", avg
ENDPROCEDURE

FUNCTION calcAvg (scores : ARRAY) RETURNS REAL
	DECLARE sum, avg : REAL
	FOR iterator <- 1 TO 15
		sum <- sum + scores[iterator]
	NEXT iterator
	avg <- sum/15
	RETURN avg
ENDFUNCTION

CALL populateArrays
CALL StudentAvg
OUTPUT "class Maths average: ", ROUND(calcAvg(ArrMaths[iterator]), 1)
OUTPUT "class Physics average: ", ROUND(calcAvg(ArrPhysics[iterator]), 1)
```