```SQL
SELECT data FROM database tables
```
- Relational Algebra (Projection, Selection, Rename, Join)
- Multiple Options/Clauses
	- Which Tables
	- Which Columns
	- Which Rows: Filter Criteria
	- Which Order

```SQL
SELECT [distinct] column(s)
FROM table(s)
WHERE condition(s)
GROUP BY column(s)
HAVING condition(s)
ORDER BY column(s) sequence
LIMIT COUNT, OFFSET
```
## Sequence

1. `FROM` → which table
2. `WHERE` → which rows
3. `GROUP BY` → aggregation
4. `HAVING` → filter on aggregated values
5. `SELECT` → which columns
6. `DISTINCT` → suppress duplicates
7. `ORDER BY` → sorting the output
8. `LIMIT/OFFSET` → pick from sequence

>SQL aggregation is **the task of collecting a set of values to return a single value**. 
>
>It is done with the help of aggregate functions, such as `SUM`, `COUNT`, and `AVG`.
>
		For example, in a database of products, you might want to calculate the average price of the whole inventory.

Related to: [[SQL]]