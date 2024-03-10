Translate between domain object & table row![[Pasted image 20231102162306.png]]

## Key features
- Programmer can work only with objects, no [[SQL]] statements in the code
	- Raw [[SQL]] queries which are written as strings that are inside the Python code
- Allows querying [[2023 Semester 2/COMPSCI235 - Software Development Methodologies/database|database]] in terms of domain model structure
- Selected objects are initially marked as being [[Persistent]], after that changes in those objects are transparently synchronized with the [[2023 Semester 2/COMPSCI235 - Software Development Methodologies/database|database]] without or with minimal explicit code being written
	- concept of [[session]]
- Framework handles the mapping of objects to the [[2023 Semester 2/COMPSCI235 - Software Development Methodologies/Relational database|Relational database]] tables, where data from the objects are actually being stored
- One way of mapping through XML descriptor files
>	#Example 
>	Java Hibernate

- Python [[SQLAlchemy]] uses explicit mapping code in Python
	- Mapper
		- what class maps to what table in [[2023 Semester 2/COMPSCI235 - Software Development Methodologies/database|database]]
		- what [[Attribute(s)]] maps to what column in [[2023 Semester 2/COMPSCI235 - Software Development Methodologies/database|database]]

![[Pasted image 20231102161727.png]]