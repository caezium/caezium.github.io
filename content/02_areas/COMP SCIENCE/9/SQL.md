

`*` is called 'wildcard'


# Structured Query Language (SQL)
is the standard query language for writing scripts to obtain information from a database.
it can
- define tables
- change tables
- add data to tables
- search for data from tables (query)
- perform calculations with data from the tables

![[02_areas/COMP SCIENCE/9/attachments/ec7eb4de6bd206a86f1247df55add02c_MD5.jpeg]]


When we write SQL, we are writing an SQL script
- list of SQL commands that performs the given task, for values to be returned
![[02_areas/COMP SCIENCE/9/attachments/4f97a8f884cf1ce153e6c81be4d8c119_MD5.jpeg]]
![[02_areas/COMP SCIENCE/9/attachments/3854fdf017b1771ed3aa279bdd8b15e3_MD5.jpeg]]
![[02_areas/COMP SCIENCE/9/attachments/db7925fb3b3e00c638e77575b7445645_MD5.jpeg]]

![[02_areas/COMP SCIENCE/9/attachments/e34956bac221cc779f0dfc7834c444d3_MD5.jpeg]]

` = - EQUAL TO`
`<> - NOT EQUAL TO`
![[02_areas/COMP SCIENCE/9/attachments/f77fd857b94f007de5b9972e2ed4a986_MD5.jpeg]]![[02_areas/COMP SCIENCE/9/attachments/edcdef82cc481b3e0edff01b620506df_MD5.jpeg]]


![[02_areas/COMP SCIENCE/9/attachments/662bb14c7ed40ff319dfc9844145ae91_MD5.jpeg]]
![[02_areas/COMP SCIENCE/9/attachments/f5d9465d74445f50c878098367d03a1c_MD5.jpeg]]

---
Recall
To convert a number to its negative in binary you have to flip all the digits then add 1.
A left binary shift will move all the binary digits to the left by one digit and the right-most digits are filled in with 0s.
An IDE provides features and the facility to code and maintain code easier, including an editor, run-time environment, error diagnostics, and translators.

## task 1
The Structured Query Language, or SQL, is the standard query language used to extract information from databases.

A primary key is needed in a database table because each record should be uniquely identifiable even if the fields are the same so that each record is able to be accessed. The primary key allows each record to be identified.


Model Answer
```
Structured Query Language (SQL) is the standard query language … … for writing scripts to obtain information from a database.

Primary keys are used to uniquely identify data in a table that could be similar to another record.
```

## task 2
Type - Text/alphanumeric because you need to use letters to represent the alphabet for the ice cream type - 'choc ice'
Flavor - Text/alphanumeric because you need to use letters to represent the alphabet for the flavor type - 'chocolate'
Size - Text/alphanumeric because you need to use letters to represent the alphabet for the size type - 'Small'
Number in stock - Integer because there can only be a whole number of stock left and you need numbers to represent quantities - '34'
Re-order level - Integer - '20'

Model Answer
```
Field 1: Type

Data type: text

Reason: as the name given to the type of ice cream is a series of characters

Sample: choc ice

Field 2: Flavour

Data type: text

Reason: as the name given to the flavour of ice cream is a series of characters

Sample: vanilla

Field 3: Size

Data type: text

Reason: as the size of the ice cream is stored as a word

Sample: Small

Field 4: NumberInStock

Data type: integer

Reason: as the number in stock will be a whole number

Sample: 56

Field 5: ReOrderLevel

Data type: integer

Reason: as the re-order level will be a whole number Sample: 24
```

## task 3
SELECT allows you to select a field to be returned from a database table
FROM allows you to specify which database table you want to use
WHERE allows you to add logical conditions to choose the specific records you want
SUM allows you to add together the sum of the selected fields

Model Answer
```
• SELECT: Fetches specified fields (columns) from a table …

… queries always begin with SELECT

• FROM: Identifies the table to use …

… queries always include FROM.

• WHERE: Includes only records (rows) in a query that match a given condition …

… WHERE is an optional command.

• SUM: Adds the values in a specified field …

… must be an integer or real field.
```

## plenary
![[02_areas/COMP SCIENCE/9/attachments/aaaf21bce2df2850f961795be99c4a85_MD5.jpeg]]
i
Miss     Mr
Sing      Ling

ii
```sql
SELECT Title, Name FROM TEACHER
WHERE Subject = 'Science'
ORDER BY Name ASC;
```

iii
```sql
SELECT Title, Name FROM TEACHER
WHERE Subject = 'Science' OR Subject = 'Mathematics'
ORDER BY Name ASC;
```


Model Answer
```
i

Miss Sing

Mr Ling

ii

SELECT Title, Name

FROM TEACHER

WHERE Subject = "Science"

ORDER BY Name;

iii

SELECT Title, Name

FROM TEACHER

WHERE Subject = "Science" OR Subject = "Mathematics"

ORDER BY Name;
```


---
part 2

## task 4
worksheet

## task 5
```sql
SELECT Type, Size FROM ICECREAM
WHERE NumberInStock > 0
ORDER BY Type;
```

```sql
SELECT SUM(NumberInStock) FROM ICECREAM;
```

```sql
SELECT COUNT(Type) FROM ICECREAM
WHERE NumberInStock < ReOrderLevel;
```
## task 6
1

```sql
SELECT FirstName, FamilyName, BedNumber FROM PATIENT;

SELECT FirstName, FamilyName, BedNumber FROM PATIENT
WHERE WardNumber <> 6;

SELECT FirstName, FamilyName, BedNumber FROM PATIENT
WHERE Arrived = '12/11/2022';

SELECT FirstName, FamilyName, BedNumber FROM PATIENT
WHERE Arrived BETWEEN '12/10/2022' AND '30/10/2022';
```
2


## plenary
![[02_areas/COMP SCIENCE/9/attachments/e29a2f90ecf5b9662272990f2e55ebac_MD5.jpeg]]

a
Fields: 5
Records: 8

b
Format Check
Presence Check



review learning
www: understood what SQL is used for and its basic operations
ebi: remember definitions and purpose of SQL and some of its statements

