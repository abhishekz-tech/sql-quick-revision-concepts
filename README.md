SQL Interview Preparation - Most Important Questions

⭐ QUESTION 1
What is SQL?

SQL stands for Structured Query Language.
Used to:
Store Data
Retrieve Data
Update Data
Delete Data

⭐ QUESTION 2
What is Database?
A collection of related data.
Examples:
Hospital System, Banking System, College System, Amazon, etc

⭐ QUESTION 3
What is Table?
A table stores data in rows and columns.

⭐ QUESTION 4
Difference Between Row and Column?
Row	Column
Horizontal Vertical
Record	    Field

⭐ QUESTION 5
Types of SQL Commands?

DDL
Data Definition Language
Used to create database objects.
CREATE
ALTER
DROP
TRUNCATE

DML
Data Manipulation Language
Used to modify data.
Commands:
INSERT
UPDATE
DELETE

DQL
Data Query Language
Command:
SELECT
Used to fetch data.

TCL
Transaction Control Language
Commands:
COMMIT
ROLLBACK

DCL
Data Control Language
Commands:
GRANT
REVOKE

⭐ QUESTION 6
CREATE DATABASE

Creates Database
Syntax
CREATE DATABASE CompanyDB;

⭐ QUESTION 7
USE DATABASE

Select Database
USE CompanyDB;

⭐ QUESTION 8
CREATE TABLE

Creates Table
CREATE TABLE Employees
(
EmpID INT,
Name VARCHAR(50),
Salary INT
);

Output
EmpID  	Name	Salary
Empty Table

⭐ QUESTION 9
SQL Data Types
INT

Stores Numbers

100
500
1000
FLOAT

Stores Decimal

50.5
99.99
VARCHAR

Stores Text

Abhishek
Mumbai
DATE

Stores Date

2026-06-22
⭐ QUESTION 10
Difference Between CHAR and VARCHAR?

Most Asked

CHAR	VARCHAR
Fixed Length	Variable Length
Faster	Saves Space

Example

CHAR(10)

Stores exactly 10 characters.

VARCHAR(10)

Stores only required space.

⭐ QUESTION 11
INSERT INTO

Adds Data

INSERT INTO Employees
VALUES
(
1,
'Abhishek',
30000
);
Multiple Records
INSERT INTO Employees
VALUES
(2,'Rahul',40000),
(3,'Priya',50000);
⭐ QUESTION 12
SELECT

Fetch Data

SELECT *
FROM Employees;

Output

EmpID	Name	Salary
1	Abhishek	30000
⭐ QUESTION 13
What does * mean?
SELECT *

Means:

Fetch All Columns

⭐ QUESTION 14
Select Specific Columns
SELECT Name,Salary
FROM Employees;

Output

Name	Salary
Abhishek	30000
⭐ QUESTION 15
WHERE Clause

Filters Records

SELECT *
FROM Employees
WHERE Salary > 30000;

Output

| Rahul | 40000 |
| Priya | 50000 |

⭐ QUESTION 16
Comparison Operators
Operator	Meaning
=	Equal
>	Greater
<	Less
>=	Greater Equal
<=	Less Equal
<>	Not Equal

Examples

WHERE Salary = 30000
WHERE Salary > 30000
WHERE Salary <> 30000
⭐ QUESTION 17
ORDER BY

Sort Data

Ascending

SELECT *
FROM Employees
ORDER BY Salary ASC;

Descending

SELECT *
FROM Employees
ORDER BY Salary DESC;
⭐ QUESTION 18
Difference Between ASC and DESC?

ASC

100
200
300
400

DESC

400
300
200
100
⭐ QUESTION 19
DISTINCT

Removes Duplicate Values

Table

Department
IT
IT
HR
HR

Query

SELECT DISTINCT Department
FROM Employees;

Output

IT

HR
⭐ QUESTION 20
LIMIT / TOP

Get First Records

MySQL

SELECT *
FROM Employees
LIMIT 5;

SQL Server
SELECT TOP 5 *
FROM Employees;

