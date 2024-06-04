- most popular [[Clustering]] method
## Algorithm
Given set of [[instance(s)]] & number of [[cluster(s)]] $k$ ([[hyperparameter(s)]]), k-means is implemented in 
### 4 steps:
1. Initial guess of the [[centroid]] of each [[cluster(s)]]
2. Assign each [[instance(s)]] to its closest [[cluster(s)]] [[centroid]] (in terms of Euclidean distance)
3. Update the [[cluster(s)]] [[centroid]] based on the assignment in **step 2**
	- you now have more information
4. go back to **step 2** & repeat until [[convergence]]
	- recalculate the [[centroid]] of your [[cluster(s)]] & re-assign
		- such that the some [[instance(s)]] are closer to other [[centroid]]
## [[K-Means Algorithm]]
![[Pasted image 20240604135959.png]]
### Complexity
- $k$ number of [[cluster(s)]]
- $n$ [[instance(s)]] (each d-dimensional vector)
- $l$ number of iterations
- ### Suggestions
	- $O(nkld)$ $\rightarrow$ product of all values
- #### Bottleneck:
	- We need to compute distance from $n$ [[instance(s)]] to $k$ [[cluster(s)]] $l$ times
- For fixed $l<<k^n$ & $k<<n$,$d<<n$ then it is almost linear in $n$
	1. $l<<k^n$ = number of iterations where it CANNOT be bigger than $k^n$ (exponential)
	2. $k<<n$ = k should be far smaller than n because you want to compress your data & only be represented with small number of examples
	3. $d<<n$
	- if all 3 assumptions hold then it is fast (almost linear)
##### Why is complexity important
- because [[Clustering]] is typically applied to large databases & [[2024 Semester 1/INFOSYS303 - Solutions Architecture/Scalability|Scalability]] is important

#compsci361example ![[Pasted image 20240604140826.png]]![[Pasted image 20240604140846.png]]![[Pasted image 20240604140903.png]]![[Pasted image 20240604140927.png]]![[Pasted image 20240604140944.png]]![[Pasted image 20240604141002.png]]![[Pasted image 20240604141023.png]]
**This algo
## Potential Problems
1. We may not be aware of how many clusters there actually are (which gives a suboptimal solution)
2. Because it is a heuristic, we may still know the exact number of clusters but our 1st step on initialisation can have a big influence on your result
Each example is assigned to one (& only one) [[cluster(s)]] $\rightarrow$ no possibility of overlapping [[cluster(s)]] or leaving unassigned examples