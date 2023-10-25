## [[Database]]
- designed for day-to-day, real-time transactional [[operations]]
- routine tasks

## Schema
- Every table is connected to another table
- Break the many-to-many relationships (Association table)
- Common [[Attribute(s)]] in one of the table, move it out & put in a table ([[3NF - 3rd Normal Form]])
- Breaking down the multivalued attribute ([[Normalisation]])
    - Faster in running queries

## SQL
- Facilitating an upcoming `INSERT,UPDATE,DELETE`
- Data consistency - data is as normalised as it can be
- Access control:
    - Data is light, so any mistake can impact all operations down the line
- Concurrency control:
    - Data can be accessed by multiple people/processes at the same time
    
    <aside> 💡 must be sequenced properly
    
    </aside>

Related to: [[OLAP - Online Analytics Processing]]