The object as row proxy:
	An object that is inside of the [[SQLAlchemy Session]], not yet corresponding to any row is said to be [[Pending]]

![[Pasted image 20231102171212.png]]
- [[Pending]] objects in the [[SQLAlchemy Session]] have not yet been flushed
- [[Flushing]] is a detail that the [[SQLAlchemy Session]] manages for us