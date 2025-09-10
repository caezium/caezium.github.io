---
draft: false
---
# Read from and write to files

Recall
A trace table is a structure to help you follow an algorithm as the variables changes to find an error or to work out what the algorithm does.
Each column is for one variable and there is an extra column for outputs.
Each row follows a change in at least one of the variables
Multiple lines of outputs will be written on multiple rows

![[Files-20241208174220761.png]]
`OPENFILE test.txt FOR READ`
`OPENFILE test.txt FOR WRITE` - a new file will be created if not found, existing data will be lost

`READFILE test.txt, line`
```
DECLARE line : STRING
DECLARE filename : STRING
INPUT filename
OPENFILE filename FOR READ

DECLARE i : INTEGER
FOR i <- 1 TO 5
	READFILE filename, line
	OUTPUT line
NEXT i

CLOSEFILE filename
```
so here the `line` variable is used to store each line read from the file

`WRITEFILE text.txt, line`
```
DECLARE filename : STRING
INPUT filename
OPENFILE filename FOR WRITE

DECLARE input : STRING
OUTPUT "input a line to save in the file"
INPUT input

WRITEFILE filename, input

CLOSEFILE filename
```

`CLOSEFILE test.txt`

``

## task 1
```
DECLARE Count : INTEGER
DECLARE Line : STRING
DECLARE Filename : STRING
Filename <- "lines.txt"
OPENFILE Filename FOR WRITE
REPEAT
	OUTPUT "text"
	INPUT Line
	WRITEFILE Filename, Line
	Count <- Count + 1
UNTIL Count = 0

OUTPUT Count, "Lines added to", Filename
```
## task 2
reading and outputting every line in the file

## task 3
```
FUNCTION CheckList(name : STRING) RETURNS BOOLEAN
	DECLARE list : STRING
	list <- "guestList.txt"

	DECLARE found : BOOLEAN
	found <- FALSE
	OPENFILE list FOR READ
	REPEAT
		DECLARE line : STRING
		READFILE list, line
		IF line = name THEN
			found <- TRUE
		ENDIF
	UNTIL EOF(line) or found

	RETURN found
ENDFUNCTION
```

## Plenary
```
DECLARE store : STRING
store <- "Test"
DECLARE file : STRING
file <- "MyFile.txt"
OPENFILE file FOR WRITE

WRITEFILE file, store

OPENFILE file FOR READ
DECLARE line : STRING
READFILE file, line
OUTPUT line
```


Review learning
WWW:
understood how to read and write using Pseudocode
EBI:
remember that for writing to files, existing data will be lost and a new file will be created