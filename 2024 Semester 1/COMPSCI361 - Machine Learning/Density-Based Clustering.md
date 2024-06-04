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
## [[DBSCAN]]
#### Main idea:
- merge all neighbouring [[core point]] to form [[cluster(s)]]
	- implements a "chain reaction" throughout the dense areas
[[cluster(s)]] contain:
- All [[core point]] that can be reached by following a sequence of [[core point]]
- [[boundary points]]![[Pasted image 20240604153043.png]]
## Pseudo Code
![[Pasted image 20240604153139.png]]

#compsci361example ![[Pasted image 20240604153546.png]]![[Pasted image 20240604153558.png]]![[Pasted image 20240604153613.png]]![[Pasted image 20240604153626.png]]![[Pasted image 20240604153639.png]]![[Pasted image 20240604153659.png]]![[Pasted image 20240604153710.png]]
## Issues
1. Finding [[cluster(s)]] for a new point is expensive you need to compute distances to $m$ core points $O(md)$, or in worst case to all training points $O(nd)$
2. Some points are not assigned to a [[cluster(s)]]
3. Ambiguity of [[boundary points]]: when these are at same distance from [[core point]] that belong to different [[cluster(s)]]![[Pasted image 20240604154224.png]]
4. Sensitive to choice of $\epsilon$ and $minNeighbours$
	- Original paper proposed to an [[elbow method]] to select $\epsilon$ based on some fixed value $k$
		- set $k$ to 4
		- set $minNeighbours$ to $k$
		- calculate and plot distances of each point to the $k$ closest neighbours
		- sort the points & plot the distances
		- look for "elbow" to set $\epsilon$![[Pasted image 20240604154658.png]]
	- Otherwise, not sensitive to initialization (except for [[boundary points]])
	-  