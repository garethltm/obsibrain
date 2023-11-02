One of the most critical tasks [[software]] applications must perform is to save & restore data

[[Persistence]] is the storage of data from working memory so that it can be restored when the application is running again

Most of the time, applications work with object-oriented systems
- Usually objects aren't [[ACID]] compliant

Object-oriented Models & Serialization![[Pasted image 20231102153010.png]]

Read or write whole objects from or to a stream of bytes, which is suitable to be streamed to a file on disk or over a network

In Python, we can use `Pickle` library
- `pickle.dump(object, outfile)`
- `object - pickle.load(infile)`
	- deserializing
	- Serializing/deserialzing $\rightarrow$ trivial
		- Not effective: file doesn't conform to the [[ACID]] properties

[[COMPSCI235 - Software Development Methodologies/database|database]] storage via a [[Relational DBMS (RDBMS)]]
