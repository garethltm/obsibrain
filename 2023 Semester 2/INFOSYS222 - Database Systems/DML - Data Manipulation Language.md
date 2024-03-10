```SQL
INSERT rows IN a table
UPDATE content IN specific column of a row in a table
DELETE rows FROM a table
```

- `INSERT` → Adding records into a table
- `UPDATE` → Editing records in a table
- `DELETE` → Deleting records from a table
```SQL
INSERT INTO <table> <"specific" columns> VALUES <values>
UPDATE <table> SET <column> = <value>
DELETE FROM <table>
```

## Add Data
1. What should be the sequence of data creation?
2. Why does the sequence matter?
    1. If you have a FK relationship can get violated if you try to add data in the child table when the parent table is missing

### Modification
- How to correct any mistakes?
    - you can `UPDATE` the table or modify it straight from the interface

### Deletion
- Get rid of any food type or food not used

    <aside> 💡 Idea of deleting from the child table then the parent table
    </aside>

Related to: [[SQL]]
