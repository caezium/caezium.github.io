


























```py
letterGrid = {'a','b','c','d','e','f','g','h'}
whiteAlive = {'P','P','P','P','P','P','P','P','R','N','B','Q','K','B','N','R'}
blackAlive = {'p','p','p','p','p','p','p','p','r','n','b','q','k','b','n','r'}
whitePos = {}
blackPos = {}

for loop assing pos values,row column

def parseInput(in):
	len = in.length()
	in = in[0]+lcase(substr(n,1,len))
	legal = False
	
	for i in letterGrid:
		if in==i:
			if findLegalMoves() --ambiguous?()
				legal = True
				return move

	wantsCheck = False
	wantsTake = False
	if move.substr(len) == '+':
		wantsCheck = True
		if len == 5:
			if in[1] == 'x':
				wantsTake = True
			else:
				return legal
		elif len != 4:
			return legal

	//check if piece alive
	owner = False //true for white, false for black
	if move[0] > 'z':
		owner = True
	alive = False
	if owner:
		for i in whiteAlive:
			if move[0] == whiteAlive[i]:
				alive = True
				break
	else:
		for i in blackAlive:
			if move[0] == blackAlive[i]:
				alive = True
				break
	if not alive:
		return legal

	
```