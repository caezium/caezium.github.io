---
draft: false
---
# [[02_areas/COMP SCIENCE/8PSEUDOCODE/Variables and Constants]]

## Green task

1.        Describe the significance of [[02_areas/COMP SCIENCE/8PSEUDOCODE/Variables and Constants]] in programming. Give examples to support your understanding.

Variables can be declared to easily changed during the execution of code, this makes programming easier and solving problems easier. Constants can be assigned so you don’t accidentally change vital values such as pi.

2.        How are variables updated in a program?

Variables in a program can be edited and updated by referencing to it and assigning it a new value.

## Amber task

1.        Write a pseudocode program for collecting a user’s first name and surnames using variables and displaying them.

```pseudocode

DECLARE first : STRING

DECLARE last: STRING

OUTPUT “first name:”

first <- INPUT

OUTPUT “last name:”

last <- INPUT

OUTPUT “hello “, first,” “, last

```

# [[02_areas/COMP SCIENCE/8PSEUDOCODE/Basic Data Types]]

## Green task

1.        Identify and define different data types used in programming.

Integer – whole numbers

Float – decimals

String – list of characters

Char – single character

Boolean – true or false

2.        Give an example where you could use each one in a school.

Integer – student no.

Float – attendance accuracy

String – name

Char – male or female

Boolean – present or absent

## Amber task

1.        Calculate the size of data files on the amber slide.

1000 students

Single student =  72 byte , 120 byte, 8 byte, 1 bit, total 1601 bits

1000 students: 200,125 bytes

## Red task

Sleep calculator

Create a pseudocode algorithm for a program to calculate how many hours per week you sleep.

Add code to your program to find the total number of hours spent sleeping in a month. Assume and average of 4.35 weeks per month.

Now find the number of days per month you sleep for!

```pseudocode

DECLARE hourspernight : INTEGER

OUTPUT “how man hours per night do you sleep?”

Hourspernight <- INPUT

DECLARE hoursperweek : INTEGER

Hoursperweek <- hourspernight * 7

OUTPUT  “You sleep ”,hoursperweek,” hours per week”

DECLARE hourspermonth : REAL

Hourspermonth = hoursperweek * 4.35

OUTPUT “you sleep “, hourspermonth, “ hours per month”

DECLARE dayspermonth : REAL

Dayspermonth <- hourspermonth / 24

OUTPUT “this equates to “, dayspermonth,” days per month”

```

# Sequence, [[02_areas/COMP SCIENCE/8PSEUDOCODE/SELECTION]] and [[02_areas/COMP SCIENCE/8PSEUDOCODE/ITERATION]]

##Green task

```pseudocode

DECLARE username : STRING

DECLARE mobilephonenetwork : STRING

OUTPUT “username?”

Username <- INPUT

OUTPUT “whats your mobile phone network?”

Mobilephonenetwork <- INPUT

DECLARE minutesUsedThisMonth : INTEGER

OUTPUT “how many minutes have you used this month?”

minutesUsedThisMonth <- INPUT

DECLARE textsUsedThisMonth : INTEGER

OUTPUT “how many texts have you used this month?”

textsUsedThisMonth <- INPUT

DECLARE bill : REAL  
bill <- minutesUsedThisMonth * 0.1 + textsUsedThisMonth * 0.05

OUTPUT “your bill this month is “,bill

DECLARE vat : REAL

Vat <- bill*0.2

OUTPUT ”your bill + VAT of 20% is “, bill+vat

```

### Additional task

```pseudocode

DECLARE amountSpent : REAL

OUTPUT “how much have you spent already?”

amountSpent <- INPUT

DECLARE bill : REAL

DECLARE discounted : REAL

IF bill <= 10 THEN

                  discounted <- bill*0.9

ELSE

                  Discounted <- bill*0.8

ENDIF

OUTPUT “your final discounted price is: “, discounted

```

## Amber task

```pseudocode

DECLARE [[[[[[[[[[[[[[[[[[speed]]]]]]]]]]]]]]]]]] : INTEGER

[[Speed]] <- INPUT

IF [[speed]] >= 75 THEN

                  OUTPUT “Issue Fine”

ELSEIF speed > 70 THEN

                  OUTPUT “Issue Warning”

ELSE

                  OUTPUT “No Action Required”

ENDIF

```

## Red Task

1.        For: a loop that can be run for a set amount of times

```

FOR count <- 1 TO 10

PRINT count

NEXT

```

WHILE: loop that can be run until a conditional thing is met, but you have to manual deduct the count.

```

While count < 10 DO

PRINT count

Count <- count+1

ENDWHILE

```

REPEAT: repeat that loop for a set amount of times, but the loop body executes before the condition is tested, so it runs at least once. Like the while loop, you have to manual deduct the count as well.

```

REPEAT

PRINT count

Count <- count +1

UNTIL count <10

```

#### Password checker

```pseudocode

DECLARE password : STRING

Password <- “what?”

DECLARE entry : boolean

Entry <- false

DECLARE attempts : INTEGER

Attempts <- 0

CONSTANT AllowedAttempts :<- 3

WHILE entry == false AND attempts < AllowedAttempts  DO

                  PRINT “please enter the password”

                  DECLARE in : STRING

                  In <- INPUT

                  IF in == password THEN

                                    Entry <- true

                  ELSE

                                    Attempts <- attempts + 1

                  ENDIF

ENDWHILE

IF entry THEN

                  PRINT “hi ”

ELSE

                  PRINT “You’ve run out of attempts”

ENDIF

```

### Review

WWW:

                  Code logic works I think

EBI:

                  Use better examples to show difference between FOR, REPEAT, and WHILE.


# Data Types – Sequencing

## Task 1

```pseudocode

CONSTANT num1 <- 10

CONSTANT num2 <- 12

OUTPUT num1+num2

```

## Task 2

```pseudocode

DECLARE age : INTEGER

DECLARE name : STRING

OUTPUT “name?”

INPUT name

OUTPUT “age?”

INPUT age

OUTPUT “Hello “, name, “ you are “, age, “ years old.”

```

## Task 3

```pseudocode

DECLARE celsius : REAL

DECLARE fahrenheit : REAL

INPUT celsius

Fahrenheit <- celsius * 1.8 +32

OUTPUT fahrenheit

```

WWW: program works I think.

EBI: task 3 ask if you want to convert C to F or F to C, instead of only C to F.


# [[02_areas/COMP SCIENCE/8PSEUDOCODE/SELECTION]]- IF

## Green Task

Write a Python program to find out whether a number is prime or not.

```

DECLARE num : INTEGER

OUTPUT "number: "

INPUT num

DECLARE prime : BOOLEAN

prime <- TRUE

IF num = 1 OR num = 0 THEN

                  prime <- FALSE

ENDIF

DECLARE count : INTEGER

DECLARE aaa : INTEGER

aaa<-SQUAREROOT(count) //i do not know the syntax for pseudocode

FOR count<-2 TO aaa

                  IF num MOD count = 0 THEN

                                    prime <- FALSE

                                    BREAK

                  ENDIF

NEXT

IF prime THEN

                  OUTPUT num," is a prime number"

ELSE

                  OUTPUT num," is not a prime number"

ENDIF

```

## Amber Task

Write a Python program to find out the divisors of a number.

```

DECLARE num : INTEGER

OUTPUT “ num:?”

INPUT num

DECLARE count : INTEGER

FOR count<-1 TO SQUAREROOT num

                  IF num MOD count == 0 THEN

                                    OUTPUT count, num DIV count

                  ENDIF

NEXT

```

## Red Task

Write a Python Program that ask the user to input a color. The program should then output a different message if the user enters the word “yellow”, “green” or, “blue”. If neither of these are entered, the program should output a different message.

```

DECLARE in : STRING

OUTPUT “input a color”

INPUT in

IF in == “yellow” OR in == “green” OR in == “blue” THEN

                  OUTPUT “correct.”

ELSE:

                  OUTPUT”wrong.”

ENDIF

```


# Python [[02_areas/COMP SCIENCE/8PSEUDOCODE/ITERATION]]

## Green task

Write a Python program to ask the user to input 100 numbers, total the values and output the total.

```pseudocode

DECLARE count : INTEGER

Count <- 0

FOR i <- 1 TO 100

                  OUTPUT “input a number”

                  DECLARE in

                  INPUT in

                  count <- count + in

NEXT i

OUTPUT count

```

```py

Count = 0

For i in range (1,101):

                  Count += int(input(“enter a number”))

Print(count)

```

## Amber task

Write a python program that uses a while loop to repeatedly ask the usr to enter a positive number. Keep asking until user enters a negative number. Then, print the sum of all the positive numbers entered.

```pseudocode

DECLARE sum : INTEGER

Sum<-0

DECLARE in : INTEGER

OUTPUT “enter a positive number”

INPUT in

WHILE in>=0 DO

Sum <- sum+in

                  OUTPUT “enter a positive number”

                  INPUT in

ENDWHILE

OUTPUT sum

```

```py

Sum = 0

In = int(input(“enter a positive number”))

While in>=0:

                  Sum+=in

                  In = int(input(“enter a positive number”))

Print(sum)

```

## Red task

Write a Python program to ask the user to input number. Count how many numbers are less than 100, and how many are more than or equal to 100. Stop when the user enters the number 0.

```pseudocode

DECLARE more : INTEGER

DECLARE less : INTEGER

More <- 0

Less <- 0

DECLARE in : INTEGER

OUTPUT “integer pls”

INPUT in

WIHLE in!=0 DO

                  IF in >= 100 THEN

                                    More <- more +1

                  ELSE

                                    Less <- less + 1

                  ENDIF

                  OUTPUT “integer pls”

                  INPUT in

ENDWHILE

OUTPUT “numbers bigger or equal to 100: ”,more

OUTPUT “numbers less than 100: “,less

```

```py

More = 0

Less = 0

In = int(input(“enter an integer pls”))

WHILE in!=0:

                  If in >= 100:

                                    More+=1

                  Else:

                                    Less+=1

Print(“numbers bigger or equal to 100:”,more,”\n”,”numbers less than 100:”,less)

```

WWW

                  Code works I think, understood how loops work

EBI

                  Do it faster. Make print results look better
# Python [[02_areas/COMP SCIENCE/8PSEUDOCODE/totaling and counting]]

## Task 2

Program that will keep letting me add money to a piggy bank until I hit 100

```pseudocode

DECLARE bank : REAL

Bank <- 0.00

WHILE bank < 100 DO

                  OUTPUT “add money”

                  DECLARE in : REAL

                  INPUT in

                  Bank <- bank + in

ENDWHILE

OUPUT bank

```

WWW: I know how to total stuff. I think my pseudocode works.

EBI: do task 3 because it’s harder.


# [[02_areas/COMP SCIENCE/8PSEUDOCODE/String handling]]
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

WWW:
	i think my code works and i did all 3 tasks
EBI: 
	write python for task 2 and task 3


# Logical and Boolean
take 2 numbers as input, n1 and n2. 
compare n1 and n2.
output a suitable message when
	- both numbers are not equal
	- which number is larger
	- which number is smaller
	- both numbers are equal

continued..
take in a third number, n3
output a suitable message when
	- all three numbers are not equal
	- all numbers are equal
```pseudocode
DECLARE n1 : INTEGER
DECLARE n2 : INTEGER
OUTPUT "input a number"
INPUT n1
OUTPUT "input another number"
INPUT n2

IF n1==n2 THEN
	OUTPUT n1," is equal to ",n2
ENDIF
IF n1!=n2 THEN
	OUTPUT n1," is not equal to ", n2
	IF n1>n2 THEN
		OUTPUT n1," is bigger than ", n2
		OUTPUT n2," is smaller than ", n2
	ELSE
		OUTPUT n1," is smaller than ", n2
		OUTPUT n2," is bigger than ", n1
	ENDIF
ENDIF



DECLARE n3 : INTEGER
OUTPUT "input a third number"
INPUT n3

IF n1==n2 AND n1==n3 THEN
	OUTPUT "all three numbers are equal"
ENDIF
IF n1!=n2 OR n1!=n3 OR n2!=n3 THEN
	OUTPUT "all three numbers are not equal"
ENDIF
```

WWW: used logical operators to check if the numbers are larger smaller or equal to each other

EBI: just use ELSE.

# [[02_areas/COMP SCIENCE/8PSEUDOCODE/nested statements]]
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

## Task 1
Inner construct : index 2
Outer construct : index 1

## Task 2
OUTPUT: a matrix/table of rows and columns inputed with the character `*`. the index 1 count variable is used to make sure the amount of rows are correct, and the index 2 is to make sure the columns are correct.

## Task 3
triangle.

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

review learning
what could you use a computer to control in your home
printer, phone, ipad.

# Subroutine - procedures and functions
procedure - subroutine performing a task **without returning** anything
function - subroutine performing a task but **returns something**
## task 2
type - procedure
name - MyProcedure
parameters - var1 int, var2 bool
```
PROCEDURE MyProcedure(Var1 : INTEGER, Var2 : BOOLEAN)
	IF Var1 < 10 AND Var2 THEN
		OUTPUT "Green"
	ELSE
		IF Var1 > 10 THEN
			OUTPUT "Blue"
		ELSE
			OUTPUT "Red"
		ENDIF
	ENDIF
ENDPROCEDURE

CALL MyProcedure(69, FALSE)
```
## task 3
```
FUNCTION whoasked RETURNS STRING
	DECLARE color
	OUTPUT "color"
	INPUT color
	RETURN color
ENDFUNCTION

FUNCTION nooneasked RETURNS STRING
	DECLARE food
	OUTPUT "food"
	INPUT food
	RETURN food
ENDFUNCTION

PROCEDURE foodcolor(color : STRING, food : STRING)
	OUTPUT color, " eggs and ", food
ENDPROCEDURE

CALL foodcolor(whoasked, nooneasked)
```

www: code works!! i know how to call subroutines in pseudocode now
ebi: even better if someone asked. make code more simple





Review learning
So far, we learned about how to declare [[02_areas/COMP SCIENCE/8PSEUDOCODE/Variables and Constants]] in pseudocode along with  data types. We also learned sequence, [[02_areas/COMP SCIENCE/8PSEUDOCODE/SELECTION]], and iterations (IF THEN, FOR loop, WHILE loop, REPEAT loop). Last lesson we learned about subroutines, procedures and functions. Procedures are subroutines that perform a set task but does not return anything. On the other hand, functions are subroutines and returns a variable.

# [[02_areas/COMP SCIENCE/8PSEUDOCODE/variable scope]] - global and local
## task 1
Global variable - the variable or constant that is accessible to all parts of the program, not declared in a subroutine.
Local variable - variable or constant that is only accessible to the subroutine that it is declared in, it is also accessible to the subroutines in that subroutine.
	if a local variable has the same name as the global variable, both variables are local. the "global" variable can only be used outside the procedure, and the local can only be used inside. the "global variable" is now a local variable , outside the procedure
## task 2
Global - Var1
Local - Var2, Param
## task 3
```
DECLARE x,y : INTEGER
DECLARE r : REAL
DECLARE colorHex : STRING
x <- 0
y <- 0
r <- 1

PROCEDURE updateColor
	OUTPUT "update color, enter the color formatted as hex"
	DECLARE in : STRING
	INPUT in
	in <- UPPER(in)

	DECLARE flag : BOOLEAN
	flag <- TRUE
	IF in[1] != '#' THEN
		flag <- FALSE
	ELSEIF LENGTH(in) != 7 THEN
		flag <- FALSE
	ELSE
		FOR i<-2 TO 7
			IF in[i] != '0' OR in[i] != '1' OR in[i] != '2' OR in[i] != '3' OR in[i] != '4' OR in[i] != '5' OR in[i] != '6' OR in[i] != '7' OR in[i] != '8' OR in[i] != '9' OR in[i] != 'A' OR in[i] != 'B' OR in[i] != 'C' OR in[i] != 'D' OR in[i] != 'E' OR in[i] != 'F' THEN
				flag <- FALSE
				BREAK
			ENDIF
		NEXT
	ENDIF
	
	

	IF !flag THEN
		OUTPUT "format incorrect, rejected"
		CALL updateColor
	ELSE
		colorHex <- in
		OUTPUT "color changed to:", colorHex
	ENDIF
ENDPROCEDURE

CALL updateColor

```

WWW: understood global and local variables
EBI: understand what will happen if variables have the same name, use pseudocode arrays to loop through if if is using hex digits/characters.


# [[02_areas/COMP SCIENCE/8PSEUDOCODE/Library Routines]]
RECALL
	3 facts: syntax in pseudocode have to be in all capitals, stuff in function brackets are parameters, the value in the parameters are arguments.
---
[[02_areas/COMP SCIENCE/8PSEUDOCODE/Library Routines]] are pre-defined subroutines that allow you to implement functionality without needing to write your own code.


Pseudocode [[02_areas/COMP SCIENCE/8PSEUDOCODE/Library Routines]]
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


WWW
	i think the code works great
EBI
	optimize the code more. maybe pre-compute the indexes of the first occurrence and calculate sum as we input.


# [[02_areas/COMP SCIENCE/8PSEUDOCODE/Maintainable Programs]]
RECALL
Libraries, [[02_areas/COMP SCIENCE/8PSEUDOCODE/Library Routines]], mod, div
routines that are predefined for you to use
mod is remainder, div is quotient

#### Meaningful identifier names
#### modules have to be divided and commented appropriately

## Task 2
No it is not maintainable.
the variable names are vague and not meaningful, change them to better names.
there are also no comments explaining what the modules/program does. add it.

## Task 3
make program from [[02_areas/COMP SCIENCE/8PSEUDOCODE/variable scope]] task 3 maintainable
```
DECLARE circleX,circleY : INTEGER
DECLARE radius : REAL
DECLARE colorHex : STRING
circleX <- 0
circleY <- 0
radius <- 1

PROCEDURE updateColor
	OUTPUT "update color, enter the color formatted as hex"
	DECLARE in : STRING
	INPUT in
	in <- UCASE(in)
	// getting new color from user, using "in" variable for input storing, uppering input so its consistent


	//flag to check if the format of the hex is correct false flag = wrong format
	DECLARE flag : BOOLEAN
	flag <- TRUE
	IF in[1] != '#' THEN
		flag <- FALSE
	ELSE
		IF LENGTH(in) != 7 THEN
			flag <- FALSE
		ELSE
			//hex first index is #, following are 0-9 or A-F, checking them here, stupid way of doing it but it works.
			FOR i<-2 TO 7
				IF in[i] != '0' OR in[i] != '1' OR in[i] != '2' OR in[i] != '3' OR in[i] != '4' OR in[i] != '5' OR in[i] != '6' OR in[i] != '7' OR in[i] != '8' OR in[i] != '9' OR in[i] != 'A' OR in[i] != 'B' OR in[i] != 'C' OR in[i] != 'D' OR in[i] != 'E' OR in[i] != 'F' THEN
					flag <- FALSE
					BREAK
				ENDIF
			NEXT
		ENDIF
	ENDIF
	
	

	IF !flag THEN
		OUTPUT "format incorrect, rejected"
		
		//rejecting and asking again
		CALL updateColor
	ELSE
		colorHex <- in
		OUTPUT "color changed to:", colorHex
	ENDIF
ENDPROCEDURE

CALL updateColor

```
WWW
	made code more readable and maintainable
EBI
	use other way of checking if its hex format so its more readable instead of using multiple ors.