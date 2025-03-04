---
draft: false
---
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
