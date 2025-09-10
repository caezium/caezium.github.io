---
draft: false
---
# Variable Scope - global and local
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
