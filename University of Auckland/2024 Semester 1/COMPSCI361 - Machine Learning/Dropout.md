We randomly [[Dropout]], set 0 to some of the weights
- causing some neurons to be useless (similar to L1 [[Regularisation]]) 
	- [[L1 & L2 regularisation]]
## How does it work?
![[Pasted image 20240607003942.png]]
becomes:
![[Pasted image 20240607003953.png]]
## Why does it work?
The nodes cannot rely on any single previous node (feature)
- Prevents too large weights
- Encourages spreading out the weights
- Forces the nodes to be more generally useful
Can be combined with other forms of [[Regularisation]] like [[L1 & L2 regularisation]] - that works on [[Loss Function]] for optimisation