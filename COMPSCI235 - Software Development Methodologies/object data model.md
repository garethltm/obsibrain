The [[object data model]] is the basis of [[Object-Oriented Database Management System (OODBMS)]]![[Pasted image 20231102155316.png]]![[Pasted image 20231102155334.png]]

- ##### Object Identity
	- Identity determines how entities are distinguished from one another
		- similar to Primary Key![[Pasted image 20231102155442.png]]
- Relationships?
	- In an [[Relational DBMS (RDBMS)]] relationships are established through matching primary key & foreign key
		- [[Relational DBMS (RDBMS)]] can only allow scalar value
- Unlike relational model, in [[object data model]] multi-valued [[Attribute(s)]] are allowed (sets)
- Class at "one" end of the [[Relationship(s)]] must hold a set of related [[Object ID (OID)]]s
- Class at "many" end of the [[Relationship(s)]] must hold [[Object ID (OID)]] of parent
- Direct extension to "many-to-many" (sets in both)![[Pasted image 20231102160612.png]]

## Advantages
1. complex objects & relationships
2. class hierarchies, inheritance
3. no impedance mismatch
4. no need for primary keys
5. no need for query language ([[s
6. 

Related to: [[COMPSCI235 - Software Development Methodologies/Relational database|Relational database]], [[Object ID (OID)]]
