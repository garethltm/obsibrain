- recursively updates the values of [[state(s)]] in the [[game tree]] as in the [[Minmax Algorithm]], while preserving values **α** , **β** for every [[state(s)]] it encounters & pruning branches accordingly
	- **α**: The best (highest) score MAX can achieve so far along the [[path(s)]] being explored
	- **β**: The best (lowest) score MIN can achieve so far along the [[path(s)]] being explored

![[Pasted image 20231023195938.png]]
![[Pasted image 20231023195954.png]]

### General Algorithm Idea
![[Pasted image 20231023200043.png]]
![[Pasted image 20231023200059.png]]
![[Pasted image 20231023200113.png]]
![[Pasted image 20231023200129.png]]
![[Pasted image 20231023200145.png]]
![[Pasted image 20231023200158.png]]
