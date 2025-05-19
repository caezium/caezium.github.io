A **database is a collection of data** that is set up in a **structured way.** It holds data about objects. *Each object is stored in a table.*

Each table is made up of **fields, which is an individual piece of data** being stored about an object, and a **record is a collection** of these fields about one object.

![[02_areas/COMP SCIENCE/9/attachments/Pasted image 20250415103521.png]]

*Why do we need a database?*
To store data about people, things and events.
Data consistency
All users access and utilize the same set of data, uniformity.


##### Single-table Database
to define a single-table database you will need to decide
- *fields* that you need
- **data types** for each field
	- text/alphanumeric: number of characters
	- character: a single character
	- boolean: one of two values, true of false, 1 or 0, yes or no
	- integer: whole number
	- real: a decimal number
	- date/time: date and/or time
- **the primary key**
	- *unique identifiers*
	- ID
	- you can have two of the same records but the primary key will make them different and separately accessible


##### Validation
Some provide auto checks while others needs to be set up by the developer.

*Validation checks are checks to make sure the data enters is correct for that field. ex. data type, format, within range*

|Validation Check|Purpose/Example|
|---|---|
|Presence|Field is not left blank|
|Format|Data matches a pattern (e.g., SN123)|
|Length|Data is a specific length (e.g., 5 characters)|
|Range|Data is within a set range (e.g., 1–100, or valid dates)|
|Type|Data is the correct type (e.g., number, date)|
|Uniqueness|Data is not duplicated (e.g., unique Show Number)|
|Check Digit|Mathematical check for numbers (e.g., barcodes, ISBN)|

---

---


recall
Computers can only read binary data.
Text can be represented with character sets that assign numeric values to each character. Some common character sets are the American Standard Code for Information Interchange and Universal character encoding.

## task 1
School ID (integer) | Name (text) | Gender (text) | Age (integer) | Occupation (text) | Nationality (text)
redacted | Mr.Mac | Male | 31 | Teacher | British
redacted | Aaron | Male | 14 | Student | Chinese
redacted | Arthur | gender-fluid | 15 | Student | Chinese
24640 | Henry | Male | 15 | Student | HK


## task 2

Answers:
![[02_areas/COMP SCIENCE/9/attachments/Pasted image 20250415105627.jpg]]
![[02_areas/COMP SCIENCE/9/attachments/Pasted image 20250415105632.jpg]]
![[02_areas/COMP SCIENCE/9/attachments/Pasted image 20250415105638.jpg]]
![[02_areas/COMP SCIENCE/9/attachments/Pasted image 20250415105648.jpg]]

## task 3
Clothing Store
Cloth ID (integer) | Type (text) | Name (text) | In-store (Date/Time) | Been Bought (boolean) | Price (Real) | Sold at (Date/time) | responsible personnel (text)





## plenary
1.
Boolean - True
Integer - 1
Text - "hello"
character - "h"
real - 1.1
Date/time - 04/15/2025

2.
A database table is a table for rows and columns. The columns are called fields, which are the specific data stored for each object. The rows are called records, which are a collection of the fields for one object.
A database's fields will have a designated data type and should have a field with a unique identifier so that data can be accessible.

3.
The primary key is used to uniquely identify each collection of data, a record for an object. This is so that even if the other fields are the of the same content, each record can still be accessed.

4.
a.
Fields: username (text), password(text), display name (text), date created (date/time), friend count (integer)

b.
the username can be the unique identifier for each record, so it can be the primary key


answer:
![[02_areas/COMP SCIENCE/9/attachments/Pasted image 20250415105726.jpg]]


review learning
www: understood database-specific terminology
ebi: think of practical database uses/fields they can use.

---
second lesson extended


recall
Databases are tables with records of data for objects with individual fields of different types of data.
Data types can be text/alphanumerical, characters, time/date, boolean, real, integer
Databases should have a primary key so duplicate records can still be separately identified.

## task 1
worksheet
## task 2
Customer ID (integer) | Registered at (date/time) | personnel ID who received the customer (integer) | phone number (integer) | email (text) | other contact methods (text) | their private data collected (text) | total spend (real) | items bought (integer) | last shopped at (date/time) |

## task 3
Student ID (integer) | Legal name (text) | nationality (text) | age (integer) | birth date (date/time) | gender (text) | Grade level (integer) | test scores (real) | enrolled classes (text) | enrolled at (date/time) | parent name (text) | parent phone number (integer) | parent email (text) | phone number (integer) | personal email (text) | school email (text) 


## plenary
1
a
a table is a collection of records, each records have data in fields about that object.

a record is a collection of data in a table's fields of an object

a field is the specific type/single piece of data collected in each record of a table.

b
text/alphanumeric: text/alphanumeric
char: b
Date/time: 04/17/2025
Integer: 4
Real: 0.4
Boolean: No


answers
1 a

• table: a collection of records … 

… where each record contains data about a similar item, e.g. a student. 

• record: a collection of fields about the same item … 

… there are the same number of fields in each record. 

• field: a single piece of data … 

… that is given a data type. 

b Four from: 

• text/alphanumeric – e.g. a description of a part

• character – e.g. S, M or L for the size of a part 

• Boolean – e.g. true or false, sold or not 

• integer – e.g. number of parts in stock 

• real – e.g. price of an item 12.99

• date/time – e.g. a date such as 18/12/2020



Review learning
www understood why need primary key
ebi specific examples of suitable primary keys for different situations