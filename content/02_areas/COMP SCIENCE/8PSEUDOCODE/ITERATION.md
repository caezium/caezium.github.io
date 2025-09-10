---
draft: false
---
## Green task

Write a program to ask the user to input 100 numbers, total the values and output the total.

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
