The object as row proxy:
	An object is [[Persistent]] when it acts like a proxy (placeholder) to a row present in the [[transaction(s)]]

![[Pasted image 20231102165944.png]]
- Row is always known as result from `SELECT` or `INSERT`
- `SELECT` leads to lookup of [[University of Auckland/2023 Semester 2/COMPSCI235 - Software Development Methodologies/database|database]] row
- `INSERT` leads to request for a free Primary Key
- [[Flushing]] moves [[SQLAlchemy Session]] objects into [[transaction(s)]]