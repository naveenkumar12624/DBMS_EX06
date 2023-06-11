# Exp-6 SET OPERATIONS.
## AIM:
To write a sql query to perform set operations on two tables.
## PROCEDURE:
### STEP 1:
create database SET_OPERATION.
### STEP 2:
create table A,B.
### STEP 3:
Insert Value to the tables.
### STEP 4:
Perform Set operations like Union,Union all,Intersect,Except.
## PROGRAM:
```sql
CREATE DATABASE SET_OPERATION;
SHOW DATABASES;
USE SET_OPERATION;
CREATE TABLE A (
  ID INT PRIMARY KEY,
  name VARCHAR(50)
);
CREATE TABLE B (
  ID INT PRIMARY KEY,
  name VARCHAR(50)
);
INSERT INTO A (ID, name) VALUES (1, 'John');
INSERT INTO A (ID, name) VALUES (2, 'Mary');
INSERT INTO A (ID, name) VALUES (3, 'David');
INSERT INTO B (ID, name) VALUES (2, 'Mary');
INSERT INTO B (ID, name) VALUES (3, 'David');
INSERT INTO B (ID, name) VALUES (4, 'Lisa');
SELECT * FROM A;

SELECT * FROM B;

SELECT * FROM A
UNION
SELECT * FROM B;

SELECT * FROM A
UNION ALL
SELECT * FROM B;

SELECT * FROM A
INTERSECT
SELECT * FROM B;

SELECT * FROM A
EXCEPT
SELECT * FROM B;
```
## OUTPUT:
![image](https://github.com/Karthikeyan21001828/DBMS_EX06/assets/93427303/202fb0df-e171-40d0-b076-e41be6a2b3f6)

![image](https://github.com/Karthikeyan21001828/DBMS_EX06/assets/93427303/6e0967b9-5c32-447d-aee6-8fa4bf633737)

![image](https://github.com/Karthikeyan21001828/DBMS_EX06/assets/93427303/18a16064-571e-4f13-a61c-95c4fe3cc606)

![image](https://github.com/Karthikeyan21001828/DBMS_EX06/assets/93427303/30baeb4f-8564-4eac-acd4-2c4a7d902b2f)

![image](https://github.com/Karthikeyan21001828/DBMS_EX06/assets/93427303/d931f7f8-d8a1-4d4c-87ce-dafe3e6d2285)

![image](https://github.com/Karthikeyan21001828/DBMS_EX06/assets/93427303/de1b03d4-220f-4229-aa9c-15fd33e4ac64)


## RESULT:
A sql query to perform set operations on two tables has been executed.
