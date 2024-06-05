$k$-nearest neighbor of an instance $x'$ are data points that have the $k$ smallest distance to $x'$
![[Pasted image 20240605095036.png]]
### Breaking ties
![[Pasted image 20240605095113.png]]
- Need to break ties:
	- Choose an odd $k$ value (does not solve every possible ties)
		- this allows us to always pick the majority vote
	- Randomly select between tied neighbors (pick either)
	- Weight the vote by distance
		- pick the closer label