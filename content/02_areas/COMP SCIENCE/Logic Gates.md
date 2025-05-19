```toc
```


#### AND gate
| A   | B   | X   |
| --- | --- | --- |
| 0   | 0   | 0   |
| 1   | 0   | 0   |
| 0   | 1   | 0   |
| 1   | 1   | 1   |
|     |     |     |
Semi circle shape
returns 1 if both inputs are 1

#### OR gate

| A   | B   | X   |
| --- | --- | --- |
| 0   | 0   | 0   |
| 1   | 0   | 1   |
| 0   | 1   | 1   |
| 1   | 1   | 1   |
caved in semi circle shape
returns 1 if one input is 1


#### NOT gate

| A   | X   |
| --- | --- |
| 0   | 1   |
| 1   | 0   |
triangle shape
outputs reversed input



#### NAND gate

| A   | B   | X   |
| --- | --- | --- |
| 0   | 0   | 1   |
| 1   | 0   | 1   |
| 0   | 1   | 1   |
| 1   | 1   | 0   |
AND gate with a small circle at the end
AND gate but adds a NOT at the end, so it reverses any AND outputs



#### NOR gate

| A   | B   | X   |
| --- | --- | --- |
| 0   | 0   | 1   |
| 1   | 0   | 0   |
| 0   | 1   | 0   |
| 1   | 1   | 0   |
OR gate with a small circle at the end
reverse OR gate outputs


#### XOR gate

| A   | B   | X   |
| --- | --- | --- |
| 0   | 0   | 0   |
| 1   | 0   | 1   |
| 0   | 1   | 1   |
| 1   | 1   | 0   |
OR gate shape with a curved line at the front
returns 1 if only one input is 1


## Logical expression
P = A AND (B OR C)
 test logical expression with a truth table

A B C, B or C, P
0 0 0  0, 0
1 0 0  0, 0
1 0 1  1, 1
1 1 0  1, 1
1 1 1  1, 1
0 0 1  1, 0
0 1 0  1, 0



![[02_areas/COMP SCIENCE/1/attachments/Pasted image 20250326155338.png]]


