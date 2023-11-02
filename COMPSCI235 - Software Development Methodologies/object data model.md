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
	- between objects in programming world & corresponding objects in [[COMPSCI235 - Software Development Methodologies/database|database]]
4. no need for primary keys
5. no need for query language ([[SQL]]), use of one programming language
6. high performance for tasks fitting the "navigational" class hierarchy
	- 1 class references another class
		- a graph of interconnected objects

## Disadvantages
1. schema changes
	- not independent
		- `CREATE`/`DROP` tables
2. lack of agreed standards
	- [[Relational DBMS (RDBMS)]] have a [[SQL]] as a standard query language
3. lack of ad-hoc querying
4. Not many programming languages support object [[COMPSCI235 - Software Development Methodologies/database|database]]

Related to: [[COMPSCI235 - Software Development Methodologies/Relational database|Relational database]], [[Object ID (OID)]]
