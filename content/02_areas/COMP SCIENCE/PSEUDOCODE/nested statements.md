---
draft: false
---

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

