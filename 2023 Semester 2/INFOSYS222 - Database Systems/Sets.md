- [[DQL - Data Query Language]] output is a set
![[Pasted image 20231016232509.png]]

```SQL
SELECT *
FROM <table>
WHERE <condition_1>
UNION
SELECT *
FROM <table>
WHERE <condition_2>
```

```SQL
SELECT <col_1>
FROM <table_1>
WHERE <condition_1>
UNION
SELECT <col_2>
FROM <table_2>
WHERE <condition_2>
```
