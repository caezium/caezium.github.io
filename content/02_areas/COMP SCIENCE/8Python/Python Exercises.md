recall
We learned about the programming development life cycle (analysis, design, coding, testing) last unit. We also learned some new pseudocode stuff like how to handle files, bubble sort, and linear search.
review
www I quickly remembered the basics of python using the resources sent by the teacher.
ebi get more comfortable and fluent in python so I can do stuff faster

---
### Exercise 1: Number guessing game
 
```py
import random

def guess():
	while True do:
	    try:
	        inGuess = int(input("\nPlease enter your guess: "))
	        
	        if inGuess<1 or inGuess>100:
	            print("!invalid guess, plase try again and enter an integer between 1-100 inclusive")
			else:
		        return inGuess
	    except:
	        print("!invalid guess, make sure you are entering an integer between 1-100 inclusive")

  
print("Welcome to the number guessing game!")
print("----------------------------------------")
print("The objective is to guess the number I'm thinking of.")
print("I will give you clues after your first guess.")

secretNumber = random.randint/91, 100)
print("I have thought of a number from 1 - 100")
numGuessed=0
guessCount=0


while numGuessed != secretNumber:
    numGuessed=guess()
    guessCount+=1

    if numGuessed < secretNumber:
        print("Guess is too low, guess higher!\n")
    else:
        print("Guess is too high, guess lower!\n")
  
print("---------------------------\nYes the number was",secretNumber,"\n good job!")
if guessCount==1:
    print("it only took you",guessCount,"guess!!")
else:
    print("it only took you",guessCount,"guesses")
```

---
### Exercise 4 Monty Hall Problem
```py
import random
random.seed()

door = ["goat","goat","car"]
random.shuffle(door)
print(door)

choice = int(input("door 1, 2 or 3? "))
choice -= 1
otherDoor = -1
goatDoor = -1

for i in range(3):
	if i!=choice:
		if goatDoor == -1 and door[i] == "goat":
			goatDoor = i
		elif otherDoor == -1 or door[i] == "car":
			otherDoor = i

switch = input("There is a goat behind door " +str(goatDoor+1)+ \
				" switch to door "+str(otherDoor+1)+"? (y/n) ")
if switch == "y":
	choice = otherDoor

if door[choice] == "car":
	print("You won a car!")
else:
	print("You won a goat!")
```


simulation
```py
import random
random.seed()

def MontyHall(times,switch):
        wins = 0
        avg = 0.0

        for i in range(times):
                door = ["goat","goat","car"]
                random.shuffle(door)
                choice = random.randint(0,2)
                otherDoor = -1
                goatDoor = -1

                for i in range(3):
                        if i!=choice:
                                if goatDoor == -1 and door[i] == "goat":
                                        goatDoor = i
                                elif otherDoor == -1 or door[i] == "car":
                                        otherDoor = i
                if switch == "y":
                        choice = otherDoor
                        
                if door[choice] == "car":
                        wins+=1
        avg = wins/times
        return avg



times = int(input("times to run simulation: "))
s = input("switch or no?")


print(MontyHall(times,s))
```