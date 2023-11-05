A schema represents any kind of structure that we are defining around the data
![[Pasted image 20231102140522.png]]![[Pasted image 20231102140555.png]]

- Defines table (relation) structures, associations, data constraints & data storage on disk
- Represented using schema diagrams
	- Table structures identifying entities (records)
	- Attributes (columns), their types, & constraints
	- [[Association]] ([[Relationship(s)]]) between tables
	- Mapping cardinalities to define the number of associations between entities![[Pasted image 20231102150658.png]]![[Pasted image 20231102150731.png]]

### KEYS in [[INFOSYS222 - Database Systems/Database Management System (DBMS)|Database Management System (DBMS)]]
- this is an [[Attribute(s)]] (column) or set of [[Attribute(s)]] (columns), which help you to uniquely identify row (tuple) in table (relation).

#### Special keys in a table
- Super Key: A set/combination of [[Attribute(s)]] (1 or more [[Attribute(s)]]) that collectively identify an [[Entity]] in an entity set
>	#Example 
>	records in a table
>		{ID, Title} for `Book`
>		{Name, Address, Website} for `Publisher`![[Pasted image 20231102151242.png]]
- Candidate Key: A minimal super key is called a candidate key. An entity set may have more than one candidate key.
>	#Example 
>	{ID} for `Book`
>	{Name, Address} for `Publisher`
>	- However, ID is already sufficient enough to be unique
- Primary Key: A primary key is one of the candidate keys chosen by the [[COMPSCI235 - Software Development Methodologies/database|database]] designer to uniquely identify the entity set