![[Pasted image 20231016012820.png]]

Related to: [[DQL - Data Query Language]]

## Motivation
1. Relational [[Data Model]]
	- Break complex data structure into simple relations
2. [[Normalisation]]
	- Move repeating information to reduce redundancy
3. [[Relationship]]
	- Connect different [[Entity]] using PK-FK linkages
> Combine data across multiple tables

```SQL
## CARTESIAN
SELECT * 
FROM <table>

SELECT * 
FROM <table_1>, <table_2>

SELECT * 
FROM <table_1> JOIN <table_2>

## INNER
SELECT *
FROM <table_1>, <table_2>
WHERE <table1_column1> = <table2_column1>

SELECT *
FROM <table_1> 
JOIN <table_2> ON <table1_column1>=<table2_column1>

## NON EQUI-JOIN
SELECT *
FROM <table_1>
INNER JOIN <table_2> ON <table1_column1>=<table2_column1>

SELECT *
FROM <table_1>
INNER JOIN <table_2> ON <table1_column1><GT,GE,LT,LE,NE,BETWEEN><table2_column1>

## OUTER
SELECT *
FROM <table_1>
LEFT OUTER JOIN <table_2> ON <table1_column1>=<table2_column1>

## MULTIPLE TABLES
SELECT *
FROM <table_1>, <table_2>, <table_3>

SELECT *
FROM <table_1>, <table_2>, <table_3>
WHERE <table1_column1> = <table2_column1> AND <table2_column2>=<table3_column2>

SELECT *
FROM <table_1>
JOIN <table_2> ON <table1_column1>=<table2_column1>
JOIN <table_3> ON <table2_column2>=<table3_column2>

## SELF
SELECT *
FROM <table_1>,<table_1>

SELECT *
FROM <table_1>,<table_1>
WHERE <table1_column1>=<table1_column2>

SELECT *
FROM <table1>
JOIN <table1> ON <table1_column1>=<table1_column2>
```