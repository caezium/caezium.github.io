---
draft: false
---
Create a program that prompts the user to either enter data, display statistics, reset data, or end program.

- If the user enters the option for entering data, they are continually prompted to input a real number until they input a 0. Once they enter a zero, they are taken back to the prompt to choose an option.
- ﻿﻿If the user enters the option for displaying statistics, the program will output the count of the numbers that have been input (not including zero), the average of those values, the maximum value, and the minimum value. Once the output is complete, they are taken back to the prompt to choose an option.
- ﻿﻿If they choose the enter more data, the new data should be considered a continuation of the old data for purposes of calculating the average and the Min/Max.
- ﻿﻿If they choose to reset the data, global variables should be reset and all previous data is lost.
- ﻿﻿If they choose to end program then the program ends with no further input/output.
- ﻿﻿If they input anything other than the 4 valid options, they are given an error message and asked again which option they choose.  

NOTE:
- ﻿﻿You MUST use subroutines to develop this program.
- ﻿﻿You MUST use selection and iteration to develop this program.
- ﻿﻿You MUST use CAIE maintainable code rules when. developing this program.

Today, you will be given the rubric with the requirements and techniques you will be measured against. You will not have this for a real task so it is important to be able to read these and find the parts of the question that lead to these requirements and techniques. Being able to convert their questions into these measurable parts is a very important skill.

Data Structures required:

- ﻿﻿Global variables
- ﻿﻿MaximumValue, MinimumValue, AverageOfValues, SelectedOption, CountOfValues, TotalOfValues

Requirements (Techniques):
R1 - Input and store option and make appropriate action based upon that option (Selection, Input/Output with prompts)
R2 - Count and Total the input values until the user inputs a 0
(Iteration, Selection, Counting, Totaling)
R3 - Calculate and Display requires statistics (Averaging, Min/Max)
R4 - Reset all appropriate variables when the option is selected (Selection, Initializing Variables)
R5 - End Program when appropriate option is selected and continue until this option is selected (Iteration and Conditional Statements)


```
//bool to control if the program runs or not
DECLARE run : BOOLEAN
run <- TRUE

//stat variables to log the data
DECLARE count, total, max, min, avg : REAL
PROCEDURE reset
	count <- 0
	total <- 0
	max <- 0
	min <- 0
ENDPROCEDURE

//reset
CALL reset
//loop for entering data and updating stats
PROCEDURE enterData
	//initial input
	DECLARE in : REAL
	OUTPUT "Enter the data. 0-exit"
	INPUT in
	//if its unchanged, first number will always be min, cannot be 0 cuz 0 is exit.
	IF min=0 THEN
		min <- in
	ENDIF
	//loop input, asking for input at the end so its easier to count
	WHILE in<>0.0 DO
		count <- count + 1
		total <- total + in
		IF max < in THEN
			max <- in
		ENDIF
		IF in < min THEN
			min <- in
		ENDIF
		OUTPUT "Enter the data. 0-exit"
		INPUT in
	ENDWHILE
ENDPROCEDURE

PROCEDURE display
	//dont display if no data or data got reset.
	IF count=0 THEN
		OUTPUT "no data entered or data got reset."
	ELSE
		avg <- total/count
		OUTPUT "total nums inputted: ",count
		OUTPUT "average: ",avg
		OUTPUT "max: ",max
		OUTPUT "min: ",min
	ENDIF
ENDPROCEDURE


//main loop, options for users
DECLARE option:INTEGER
WHILE run=TRUE DO
	//options.
	OUTPUT "1-enter data 2-display stats 9-reset 0-exit"
	INPUT option
	IF option=1 THEN
		CALL enterData
	ELSE
		IF option=2 THEN
			CALL display
		ELSE
			IF option=9 THEN
				CALL reset
			ELSE
				IF option=0 THEN
					//run flag set to false, while loop auto exterminates
					OUTPUT "aborting program"
					run <- FALSE
				ELSE
					OUTPUT "invalid option"
				ENDIF
			ENDIF
		ENDIF
	ENDIF
ENDWHILE
```