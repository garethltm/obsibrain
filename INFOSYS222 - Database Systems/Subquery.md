# Table vs Subquery
- Table is a matrix (rows & columns)
- [[DQL - Data Query Language]] output is also a matrix
- Subquery: [[DQL - Data Query Language]] output acting like a Table
- Executed before main [[DQL - Data Query Language]]
- Allows nesting
```SQL
SELECT *
FROM (SELECT <column>
	 FROM <table>
	 WHERE <condition>)
```
# Motivation
- Use a snapshot of table as a table
- Encapsulate query complexity into a black box
- Evaluate conditions based on subquery output
	- Use as a Scalar Value (Single Row-Column output)
	- Use as a List (Multi-Row Single Column output)
	- Use as a decision criteria (No/Some values)

```SQL
SELECT *
FROM <table>
WHERE <condition>

<col>=<subquery output>
<col> IN <subquery output>
```

```SQL
SELECT *
FROM <table_1>
WHERE EXISTS (
	SELECT *
	FROM <table_2>
	WHERE <condition>
)
```