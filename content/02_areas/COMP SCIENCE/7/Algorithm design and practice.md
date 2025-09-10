---
draft: false
---
**algorithm - a series of sequential instructions to solve a problem or perform a task**

# Recall
![[Algorithm design and practice-20241105100144401.png]]
```
Password <- ""
WHILE Password <> "rE5Bh9dP" DO
	OUTPUT "Enter password"
	INPUT Password
ENDWHILE
OUTPUT "Correct password"
```

```
DECLARE cost1, cost2 : REAL
OUTPUT "item 1 cost:"
INPUT cost1
OUTPUT "item 2 cost:"
INPUT cost2

DECLARE total : REAL
total <- cost1+cost2
IF total > 10.0 THEN
	OUTPUT "sorry, too much"
ELSE
	OUTPUT "change due from 10.00"
	OUTPUT 10.0-total
ENDIF
```


## Green Task
![[Algorithm design and practice-20241105101554803.png]]
```
DECLARE num : INTEGER
INPUT num
DECLARE count : INTEGER
FOR count <- 0 TO num
	IF count MOD 2 = 0 THEN
		OUTPUT count
	ELSE
		OUTPUT "boo"
	ENDIF
NEXT count
```
![[Algorithm design and practice-20241105102316061.png]]
```
DECLARE in : STRING
in <- "what"
WHILE in <> "hug" DO
	OUTPUT "hug me"
	INPUT in
ENDWHILE
OUTPUT "thanks"
```

## Amber task
![[Algorithm design and practice-20241105103709498.png]]
```
DECLARE in1, in2 : INTEGER
OUTPUT "input number"
INPUT in1
OUTPUT "input number"
INTPUT in2
DECLARE big, small : INTEGER
IF in1>in2 THEN
	big <- in1
	small <- in2
ELSE
	big <- in2
	small <- in1
ENDIF

DECLARE count
FOR count <- small TO big
	OUTPUT count
NEXT count
```
![[Algorithm design and practice-20241105104129369.png]]
```
DECLARE l1,l2,l3 : INTEGER
DECLARE n1,n2,n3 : STRING
INPUT n1
INPUT n2
INPUT n3
l1 <- LENGTH(n1)
l2 <- LENGTH(n2)
l3 <- LENGTH(n3)
IF l1 > l2 THEN
	IF l1>l3 THEN
		OUTPUT l1
	ELSE
		OUTPUT l3
	ENDIF
ELSE
	IF l2 > l3 THEN
		OUTPUT l2
	ELSE
		OUTPUT l3
	ENDIF
ENDIF
```
variation
```
DECLARE l1,l2,l3 : INTEGER
DECLARE n1,n2,n3 : STRING
INPUT n1
INPUT n2
INPUT n3
l1 <- LENGTH(n1)
l2 <- LENGTH(n2)
l3 <- LENGTH(n3)
IF l1 > l2 THEN
	IF l1>l3 THEN
		OUTPUT n1
	ELSE
		OUTPUT n3
	ENDIF
ELSE
	IF l2 > l3 THEN
		OUTPUT n2
	ELSE
		OUTPUT n3
	ENDIF
ENDIF
```

## red task
![[Algorithm design and practice-20241105104412354.png]]
```
DECLARE first, last : CHAR
DECLARE word : STRING
INPUT word
first <- word[0]
last <- word[LENGTH(word)-1]
OUTPUT first, last
```
variation
```
DECLARE first, last : CHAR
DECLARE word : STRING
INPUT word
first <- word[1]
last <- word[LENGTH(word)-2]
OUTPUT first, last
```


### Review learning
www
know how to flow chart loops
ebi
understand how to write stuff in the structured diagram better