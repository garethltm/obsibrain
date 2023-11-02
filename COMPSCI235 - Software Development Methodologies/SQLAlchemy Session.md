![[Pasted image 20231102165121.png]]
- The Session object is the public interface for the [[Object Relation Mapping (ORM)]]
- Establishes all [[COMPSCI235 - Software Development Methodologies/database|database]] conversations through internal explicit [[transaction(s)]]
	- what a Session does
- "Holding zone" for objects during the Session's lifespan
	- maintains an active reference to the set of all mapped entities which are present in memory
		- why it is done
- The session objects are proxies for table rows
	- holding zones are placeholders where the [[Object Relation Mapping (ORM)]] fetches table rows & places them into [[SQLAlchemy Session]] object
- Unit of Work:
	- lazily flushes (when you commit an optimisation feature) only those rows/columns that have changed, ordering them to maintain consistency
![[Pasted image 20231102165146.png]]

- Objects, when associated with a Session are proxies for rows, represented uniquely on primary key identity
	- Identity Mapping pattern, a dictionary in practice
>	#Example 
>	Dictionary:
>	PrimaryKey, Value: Reference to object in memory
- Changes to objects maintained by Session are tracked
	- We have to frequently push out changes of objects to the [[COMPSCI235 - Software Development Methodologies/database|database]]
		- Before we do a query
			- So that we get the latest data from the [[COMPSCI235 - Software Development Methodologies/database|database]]
		- When the user issues an explicit commit or a [[transaction(s)]] finishes
	- This is called **flushing** of pending changes
		- `autoflush = True`
- Several possible Session object states:
	1. [[Persistent]]
	2. [[Expired]] 
	3. [[Transient]] 
	4. [[Pending]]
	5. (Detached)