---
draft: false
---
#### Meaningful identifier names
#### modules have to be divided and commented appropriately

## Task 2
No it is not maintainable.
the variable names are vague and not meaningful, change them to better names.
there are also no comments explaining what the modules/program does. add it.

## Task 3
make program from variable scope task 3 maintainable
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