---
draft: false
---
![[Test Data-20241126103417685.png]]

![[Test Data-20241126103648629.png]]


Recall: 
bubble sort: takes first 2 values then compares theme. if they are wrong way around, swap them. then it takes the second and third values. it repeats until it goes all the way through the list. then after it has worked all the way through the list once, it repeats from the first and second again.
it is called bubble sort because it acts like a bubble moving across all the elements to the end then starting again.


# task 1
You should test your programs so that they works and meets the requirements. Using the 4 types of test data you can make sure almost all data that might be inputted by users and taken into consideration.
Range check - checks range
Length check - checks the length
Type check - checks the data type
Presence check - make sure the data isn't null or empty
Format check - check the format
Check digit - checks the digits


# task 2
there are 4 types of data that are used as test data when testing programs
normal data - valid data that meets the requirements
abnormal data - invalid data
Extreme data - data that is valid and on the edge of the acceptable values
Boundary data - data that is on the outer edge of the acceptable values. some are valid some are not. 

# task 3
Chess
Normal data - normal chess notations of moves that are legal and can be moved like that without any checks that will happen if that piece is moved.
ex. at the start of the game e4.

Abnormal data- invalid chess notations of pieces that do not exist, is moved illegally, or will reveal a check once moved
ex. z9

Extreme data - special moves such as en passent, pawn promotion, and castling
ex. O-O or O-O-O

Boundary data - moves that are valid and the piece moved are able to go there but reveals a check on their own king.

# plenary
![[Test Data-20241126105354956.png]]
`>=1 AND <=10`
`NOT >=1 OR NOT <=10`
`1 OR 10`
`(<1 AND >(1-1)) OR ()>10 AND <(10-1))`

Review learning
www: understood why you need to test programs with different types of test data
ebi: understand better extreme data and boundary data.