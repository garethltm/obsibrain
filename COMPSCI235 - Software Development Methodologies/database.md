A [[COMPSCI235 - Software Development Methodologies/database|database]] stores data persistently
- any change to the [[COMPSCI235 - Software Development Methodologies/database|database]] is permanent - it is going to stay somewhere
>	#Example 
>	in files on disk

Databases come in many forms
1. Structural relational database
>	#Example 
>	MySQL, Postgres, SQLite

2. Unstructured 'NoSQL' databases
>	#Example 
>	MongoDB, Redis (no SQL queries)

- [[COMPSCI235 - Software Development Methodologies/Relational database|Relational database]]

A [[COMPSCI235 - Software Development Methodologies/database|database]] is an organized collection of inter-related data that models some aspect of the real-world

#### Why databases?
- Store our data in flat files
- Read & Writes to flat files are non-trivial
	- We need to parse the files each time we want to read/update records
		- you also need to know the structure of the file
		- parse the whole file, where you need to bring the entire file to memory - make changes & write back to file
- Storage of data in files
- Other Problems:
	- Redundancies
		- You need to update more columns when you want to make some changes
	- Inconsistencies - potentially caused by Redundancies
		- some places are not the same
	- Security - Who has access?
	- Isolation - When there is concurrent multi-user access
	- Atomicity of updates
	- Durability

