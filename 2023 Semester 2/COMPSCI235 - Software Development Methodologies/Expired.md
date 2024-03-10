they are not linked to any [[transaction(s)]]

The object as row proxy:
	With no [[transaction(s)]] present, the state of objects is [[Expired]]. There is no view of the [[2023 Semester 2/COMPSCI235 - Software Development Methodologies/database|database]] other than via a [[transaction(s)]]

![[Pasted image 20231102170744.png]]
- This happens after a commit of the [[SQLAlchemy Session]], which finalizes a [[transaction(s)]]
- Now all changes are [[Persistent]], but the objects need to be refreshed in memory