# SQL Revision

## Structured query language
DML (Data manipulation language) – Select, insert, update, delete  
DDL (Data definition language) – Create, alter, drop, truncate  
DCL (Data control language) – Grant, revoke  
TCL (Transaction control language) – Commit. Rollback, save-point  

## Data Types
#### VARCHAR  
Adaptable to different lengths of characters. Records MAX size  
#### CHARACTER or CHAR  
Data must be at a fixed length. Fixed amount of space used.  
#### INT  
Holds a whole number/integer value (see also bigint, smallint and tinyint) positive or negative  
#### DATE or TIME or DATETIME  
Stores date time or both date and time  
#### DECIMAL or NUMERIC  
Fixed precision and scale (digits to right of decimal point) numbers  
#### BINARY  
Use to store binary data such as an image or file  
#### FLOAT  
Scientific use (very large numbers)  
#### BIT  
Equivalent to binary (0.1 or NULL)  

## Wildcards in SQL
Wildcards can be used as a substitute for any other character in a string when using the LIKE operator   
% = A substitute for zero or more characters, means any number of characters   
_ = A substitute for a single character, refers to a specific number of characters    
[charlist] = Sets and ranges of characters to match i.e. LIKE [ABC]% This will bring back anything starting with any of those letters   
[^charlist] = Sets and ranges of characters that don’t match i.e. LIKE[^ABC]% This will bring back anything that does not start with those letters.  

## Arithmetic operators in SQL
+ Add (can be used on DATETIME columns)  
- = Subtract (can be used on DATETIME columns)  
* = Multiply   
/ Divide   
% Percentage (Modulo)   

DESC = Descending   
ASC = Ascending  

## Aggregate functions in SQL
SUM = SUM(OrderTotal) for the grand total of a column for all rows selected   
AVG = AVG(UnitPrice) for the average of a column for all rows selected   
MIN = MIN(UnitPrice) for the smallest value in a column for all rows selected  
MAX = MAX(UnitPrice) for the largest value in a column for all rows selected   
COUNT = COUNT for the number of NOT NULL rows selected. If * then all rows are counted, regardless of NULL/NOTNULL.  

## SQL Commands
SELECT <Column name> =  What data to select   
FROM <Name> = Selects from chosen path  
WHERE <Column name> = Adds variables to query  
Create database <Name> = Creates a database
Create table <Name> = Creates a table
AS = Provides an alias for a column  
SP_HELP <Name> = Displays the information and what data types the file uses  
ALTER TABLE <Name> = Can be used to RENAME, MODIFY, ADD or DROP columns   
ADD <Name> = Adds something to the file   
RENAME <Name> = Renames something in the file  
MODIFY <Name> = Modifies something in the file  

## How to set up a table
USE my_db;  
CREATE TABLE film_table  
(  
film_name VARCHAR(50),   
film_type VARCHAR (20),  
date_of_release DATE  
Director VARCHAR (40),  
Writer VARCHAR (40),   
Star DECIMAL (2,1),   
Film_Language VARCHAR (50),     
Official_Website VARCHAR (100),  
Plot_Summary VARCHAR (255),  
)  
