---
draft: false
---
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
