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
## Density-Based Spatial [[Clustering]] with applications with [[Noise]] algorithm (DBSCAN)
has 2 parameters:
- $\epsilon$: distance
