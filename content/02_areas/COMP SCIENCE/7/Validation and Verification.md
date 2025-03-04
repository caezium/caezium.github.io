---
draft: false
---
# Validation
validation is checking data to make sure it is in the correct format or within set bounds.
Range check - checks range
Length check - checks the length
Type check - checks the data type
Presence check - make sure the data isn't null or empty
Format check - check the format
Check digit - checks the digits



Recall
bubble sort: takes first 2 values then compares theme. if they are wrong way around, swap them. then it takes the second and third values. it repeats until it goes all the way through the list. then after it has worked all the way through the list once, it repeats from the first and second again.
it is called bubble sort because it acts like a bubble moving across all the elements to the end then starting again.

# task 1
validation is checking data to make sure it is in the correct format or within set bounds.
Range check - checks range
Length check - checks the length
Type check - checks the data type
Presence check - make sure the data isn't null or empty
Format check - check the format
Check digit - checks the digits


# task 2
examples
Range check: make sure age is in the range
Length check: length of password enough
Type check: name input boxes to check if you actually entered a name
Presence check: on forms make sure didn't submit nothing
Format check: dates
Check digit: can be used to make sure the data isn't corrupted

# task 3
check digit is used to make sure the data transmitted is correct.
ex. on some barcodes the last digit is the sum of all other digits and the system recaulcates the check digit to verify the data. usually barcodes get the odd and even positioned digits separately. then they times the odd digits by some number like 3, then they add that result with the even digits. then they find the smallest number that when added to the result makes it a multiple of 10. this smallest number is the check digit. using a very specific calculation/check like this can help validate the data better.
check digit helps prevent incorrect data from being processed.


# plenary
28.range check
29.presence check



# Verification
# task 1 and 2
verification - check if the data you copied or entered is correct
visual check - checks if the data is the same as the data that is stored
	ex. checking passwords
double entry check - enter the data again and see if it is the same as the first entered
	ex. entering emails addresses or new passwords twice to make sure they are right
# task 3
```

OUTPUT "username"
DECLARE user : STRING
INPUT user
WHILE LENGTH(user)<5 DO
	OUTPUT "username has to be with a minimum length of 5 characters, pls try again"
	INPUT user
ENDWHILE


OUTPUT "date of birth"
INPUT date
WHILE SUBSTRING(date,1,2).GetDataType() <> String OR SUBSTRING(date,3,1)<>"/" OR SUBSTRING(date,4,2).GetDataType() <> String OR SUBSTRING(date,6,1)<>"/" OR SUBSTRING(date,7,4).GetDataType() <> String DO
	OUTPUT "data has to be formatted as NN/NN/NNNN, pls try again"
	INPUT date
ENDWHILE

OUTPUT "type of character, elf, fairy, gnome, magician"
INPUT character
in<-UCASE(character)
DECLARE flag : BOOLEAN
flag <- TRUE
WHILE flag DO
	IF character = "ELF" OR character="FAIRY"OR character="GNOME"OR character="MAGICIAN" THEN
		flag<- FALSE
	ELSE
		OUTPUT "type of character, elf, fairy, gnome, magician"
		INPUT character
	ENDIF
ENDWHILE


DECLARE strength:INTEGER
OUTPUT "strength 1-5"
INPUT strength
WHILE strength.GetDataType()<>Integer OR strength<1 OR strength>5 DO
	OUTPUT "strength 1-5"
	INPUT strength
ENDWHILE

OUTPUT "starting health, 10 minus the starting strength"
DECLARE health:INTEGER
INPUT health
WHILE health <> 10-strength DO
	OUTPUT "starting health, 10 minus the starting strength"
	INPUT health
ENDWHILE

```

WWW:know the two types of verification
EBI: more optimized/shorter code 

# plenary
verification is used to check if the data you copied or entered is correct