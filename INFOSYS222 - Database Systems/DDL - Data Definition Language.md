``` SQL
CREATE database
CREATE database users
CREATE database tables
ALTER database tables (add/modify columns)
DROP database tables
TRUNCATE database tables
```

- `CREATE` → Adding new table in DB
- `ALTER` → Edit table definition in DB
- `DROP` → Delete table from DB
```SQL
CREATE TABLE <table> (<column definitions>)
ALTER TABLE <table> {rename|add|drop}
DROP TABLE <table>
```

## VIEW
- cannot be updated directly
- just extracting content from the table
- they do not hold any data
- dynamic table, which is constructed at runtime depending what the query definitions are

```SQL
CREATE VIEW <view> AS
		SELECT *
		FROM <table_1>


-- applying projection of what we want to see specifically
CREATE VIEW <view> AS
		SELECT <col_1>, <col_2>
		FROM <table_1>
		WHERE <condition>

DROP VIEW <view>
```

## INDEX
- more efficient way of looking for data - limiting your scope of search by splitting your data (like merge sort, finding the midpoint)
- they are usually sorted
- every time you create an index, you have to create another space in the DB to store the sorted list - which takes up [[INFOSYS222 - Database Systems/Database]] space

<aside> 💡 useful for large table/frequently used columns </aside>

```SQL
CREATE INDEX <index>
ON <table> (<column>)

CREATE UNIQUE INDEX <index>
ON <table> (<col_1>, <col_2> DESC)

DROP INDEX <index>
```
- every time you create a PK, there is already an index associated with it - you don’t have to create an index for the column
- you can limit using `WHERE` clause - which can limit the size of the index

## TRIGGER
- A [[DML - Data Manipulation Language]] that depends on other [[DML - Data Manipulation Language]]
- creating triggers when something happens in a table
```SQL
CREATE TRIGGER <trigger>
[BEFORE|AFTER]
[INSERT|UPDATE|DELETE]
OF <table>
BEGIN <action>;
END

DROP TRIGGER <trigger>
```

# Adding Tables
1. What should be the sequence of creation?
2. What data types would be suitable?
3. What are the relevant constraints?
4. How should we enforce dependency?
    1. each of the FK is linked to the PK of the parent table
![[Pasted image 20231016233212.png]]
Default constraints that come with is the PK/FK: where it cannot be null and must be unique

In this context, we create the tables in this order:

1. Episode
2. Type
3. Food
4. EpisodeFood

<aside> 💡 Its good to create it in a sequence where you don’t have to go back & alter the existing ones </aside>

### Modifications

- How many times was a food mentioned in the episode
- Implement Season-Episode key concept: S05E02
    - this means that the Season (ID) & Episode would both be a PK which becomes a composite key

Related to: [[SQL]]
