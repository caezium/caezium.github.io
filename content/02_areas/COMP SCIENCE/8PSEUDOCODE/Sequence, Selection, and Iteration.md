---
draft: false
---

## Green task

```pseudocode

DECLARE username : STRING

DECLARE mobilephonenetwork : STRING

OUTPUT “username?”

INPUT username

OUTPUT “whats your mobile phone network?”

INPUT mobilephonenetwork

DECLARE minutesUsedThisMonth : INTEGER

OUTPUT “how many minutes have you used this month?”

INPUT minutesUsedThisMonth

DECLARE textsUsedThisMonth : INTEGER

OUTPUT “how many texts have you used this month?”

INPUT textsUsedThisMonth

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

DECLARE speed : INTEGER

Speed <- INPUT

IF speed >= 75 THEN

                  OUTPUT “Issue Fine”

ELSE
	IF speed > 70 THEN
	    OUTPUT “Issue Warning”
	ELSE
        OUTPUT “No Action Required”
	ENDIF
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

WHILE count < 10 DO

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

                  INPUT in

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