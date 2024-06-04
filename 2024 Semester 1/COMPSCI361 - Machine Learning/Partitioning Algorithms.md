- [[k-Means]] is a partitioning algorithm
- Partitioning a database D of n [[instance(s)]] into a set of $k$ [[cluster(s)]], such that within-cluster variation (the sum of squared distances of the [[instance(s)]] to the [[cluster(s)]] centers) is minimized
	$$
	SSE = \sum_{c=1}^{k} \sum_{x \in C_c} \text{dist}(x - w_c)^2 
	$$
- where $w_c$ is the centroid or medoid of [[cluster(s)]] $C_c$
- Given $k$, find a partition of $k$ [[cluster(s)]] that optimizes the chosen partitioning criterion
	- Global optimum: exhaustively enumerate all partitions $\rightarrow$ Expensive
	- Local optimum: heuristics, such as [[k-Means]] (not guaranteed correct solution/[[Optimal]] solution)
Suitable for detecting non-overlapping spherical [[cluster(s)]] of similar size & density
There are other types of [[Clustering]] algorithms, such as [[Density-based Clustering]] & hierarchical [[Clustering]]