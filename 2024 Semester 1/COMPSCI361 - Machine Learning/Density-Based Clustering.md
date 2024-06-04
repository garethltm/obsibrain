- [[cluster(s)]] are defined by "dense" regions
- [[instance(s)]] in non-dense regions don't get clustered
	- Not trying to "partition" the space
- Sparse doesn't mean that it is not a cluster
[[cluster(s)]] can be non-convex
#compsci361example 
	Elephant clusters affected by vegetation, mountain, rivers, water access,...
	high crime regions etc..
It's (almost) non-parametric [[Clustering]] method
- no fixed number of [[cluster(s)]] $k$
	- doesn't assume that you have to give a number of [[cluster(s)]]
		- it detects the number of [[cluster(s)]]
	- [[cluster(s)]] can become more complicated with more data

has 2 parameters:
- $\epsilon$: distance we use to decide if another point is a "neighbour"
- $minNeighbours$: number of neighbours needed to say a region is "dense"![[Pasted image 20240604152658.png]]
#### Main idea:
- merge all neighbouring [[core point]] to form [[cluster(s)]]
	- implements a "chain reaction" throughout the dense areas
[[cluster(s)]] contain:
- All [[core point]] that can be reached by following a sequence of [[core point]]
- All non-core neighbours of [[core point]] (boundary points)
	- points that are not [[core point]] but are edges of the [[cluster(s)]] (boundary)![[Pasted image 20240604153043.png]]
## Pseudo Code
![[Pasted image 20240604153139.png]]

#compsci361example ![[Pasted image 20240604153546.png]]![[Pasted image 20240604153558.png]]![[Pasted image 20240604153613.png]]![[Pasted image 20240604153626.png]]![[Pasted image 20240604153639.png]]![[Pasted image 20240604153659.png]]![[Pasted image 20240604153710.png]]