---
draft: false
---
[[Flowcharts]] are a way in which algorithms and processes may be shown graphically. **remember to draw arrows -> !**
![[Flowcharts-20241029103438136.png]]


## [[programming development life cycle]]
There are four stages in the program [[programming development life cycle]]
- Analysis
	- identify the problem
	- Abstract and decompose the problem.
	- Identify the requirements
- Design
	- consider how the program will be designed
	- overall structure and individual algorithms that may be used
	- /decomposition
- Coding/development
	- producing the program
	- iterative testing - test the programs as they are developed
- Testing
	- test the program
	- list out test data with their expected results and test if the program outputs the expected result.
	- fix the errors and re-test.


- Abstraction, certain characteristics are removed so that you focus on the main and important characteristics.
- Decomposition, a large problem is broken down into smaller tasks.
- Algorithm design, a problem is broken into a series of logical steps called an algorithm, the steps are ran one by one and solves the problem.

---
All computer systems are made up of sub systems.

[[Sub Systems and Structured Diagrams|Structured Diagrams]]
uses boxes and branches
each part of the problem is broken down again and again.
![[Sub Systems and Structured Diagrams-20241029103251132.png]]
part of design process.

need
- input
- process
- output


---
sorting : sorting content into orders

bubble sort: takes first 2 values then compares theme. if they are wrong way around, swap them. then it takes the second and third values. it repeats until it goes all the way through the list. then after it has worked all the way through the list once, it repeats from the first and second again.  
it is called bubble sort because it acts like a bubble moving across all the elements to the end then starting again.




Linear search examines items one by one in a list and checks them one by one to see if the item has been found. This search is very easy to make but very slow because its time complexity is O(n), meaning that in the worst case scenario, the item is on the end of the list and you would have to loop through the whole list to find it.
sequentially


---
# validation verification test data
You should test your programs so that they works and meets the requirements. Using the 4 types of test data you can make sure almost all data that might be inputted by users and taken into consideration.  

validation is checking data to make sure it is in the correct format or within set bounds.
Range check - checks range  
Length check - checks the length  
Type check - checks the data type  
Presence check - make sure the data isn't null or empty  
Format check - check the format  
Check digit - checks the digits

verification - check if the data you copied or entered is correct  
visual check - checks if the data is the same as the data that is stored  
ex. checking passwords  
double entry check - enter the data again and see if it is the same as the first entered  
ex. entering emails addresses or new passwords twice to make sure they are right

Test data types
normal: accepted valid
abnormal: invalid
extreme: on the edge of valid data
boundary: on the edge and slightly out of edge data



---
# trace tables

A trace table is a structure to help you follow an algorithm as the variables changes to find an error or to work out what the algorithm does.  
Each column is for one variable and there is an extra column for outputs.  
Each row follows a change in at least one of the variables  
Multiple lines of outputs will be written on multiple rows






trace table first line????,,,,....