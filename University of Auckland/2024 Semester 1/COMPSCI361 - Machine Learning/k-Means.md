- most popular [[Clustering]] method
## Algorithm
Given set of instance & number of [[cluster(s)]] $k$ ([[hyperparameter(s)]]), [[k-Means]] is implemented in 
### 4 steps:
1. Initial guess of the [[centroid]] of each [[cluster(s)]]
2. Assign each instance to its closest [[cluster(s)]] [[centroid]] (in terms of [[Euclidean distance]])
3. Update the [[cluster(s)]] [[centroid]] based on the assignment in **step 2**
	- you now have more information
4. go back to **step 2** & repeat until [[convergence]]
	- recalculate the [[centroid]] of your [[cluster(s)]] & re-assign
		- such that the some instances are closer to other [[centroid]]
## [[k-Means]]
![[Pasted image 20240604135959.png]]
### Complexity
- $k$ number of [[cluster(s)]]
- $n$ instances (each d-dimensional vector)
- $l$ number of iterations
- ### Suggestions
	- $O(nkld)$ $\rightarrow$ product of all values
- #### Bottleneck:
	- We need to compute distance from $n$ instances to $k$ [[cluster(s)]] $l$ times
- For fixed $l<<k^n$ & $k<<n$,$d<<n$ then it is almost linear in $n$
	1. $l<<k^n$ = number of iterations where it CANNOT be bigger than $k^n$ (exponential)
	2. $k<<n$ = k should be far smaller than n because you want to compress your data & only be represented with small number of examples
	3. $d<<n$
	- if all 3 assumptions hold then it is fast (almost linear)
##### Why is complexity important
- because [[Clustering]] is typically applied to large databases & [[University of Auckland/2024 Semester 1/INFOSYS303 - Solutions Architecture/Scalability|Scalability]] is important

#compsci361example ![[Pasted image 20240604140826.png]]![[Pasted image 20240604140846.png]]![[Pasted image 20240604140903.png]]![[Pasted image 20240604140927.png]]![[Pasted image 20240604140944.png]]![[Pasted image 20240604141002.png]]![[Pasted image 20240604141023.png]]
**This algorithm will return the best [[Clustering]] result for k=n, because every node will be assigned to itself**
## Potential Problems
1. We may not be aware of how many clusters there actually are (which gives a suboptimal solution)
2. Because it is a heuristic, we may still know the exact number of clusters but our 1st step on initialisation can have a big influence on your result
Each example is assigned to one (& only one) [[cluster(s)]] $\rightarrow$ no possibility of overlapping [[cluster(s)]] or leaving unassigned examples
## Potential Fix (in a predictive setting)
- Assumes you know number of [[cluster(s)]] k
	- if you don't know, you can define a function which sums up the distances from your instance from each [[cluster(s)]] to the cluster centre (within cluster variance)
- [[k-Means]] is guaranteed to converge when using [[Euclidean distance]]
	1. you can forget about all instance that belong to your [[cluster(s)]]. Your cluster centroid is like a pillar to your [[cluster(s)]]
	2. you can compute distances for that new test instances to all existing [[cluster(s)]] centres, choose the one closest to you in terms of [[Euclidean distance]]
Not all [[Clustering]] algorithms can be applied in a predictive manner to a new test instance, some only work in a valid descriptively only for the data set you have obtained.
## Behaviour/Assumptions
- Given a new (test) example
	- Assign it to the nearest ([[cluster(s)]]) center to [[cluster(s)]] it
- Each example is assigned to one (& only one) [[cluster(s)]]
	- No possibility of overlapping [[cluster(s)]] or leaving examples unassigned (outliers)
- It may converge to [[suboptimal]] solution (sensitive to initialization & outliers)
- Assumes you know the number of [[cluster(s)]] $k$
	- Lots of heuristics to pick $k$ ([[elbow method]]), none satisfying
	- [[Cross-Validation (CV)]]
## What is [[k-Means]] doing?
We can interpret [[k-Means]] steps as minimizing an objective
- Total sum of squared distances from each example $x_i$ to its [[cluster(s)]] center (squared L2 norm)$$f(w_1, \ldots, w_k, \hat{y}_1, \ldots, \hat{y}_n) = \sum_{i=1}^{n} \| w_{\hat{y}_i} - x_i \|_2^2$$
- $w_{\hat{y}_i} - x_i$ = minimizes in terms of chosen centres = because we are always refining the centres to represent the mean/ average/best point that represents
#### Steps
- minimize $f$ in terms of the $\hat{y}_i \in (1,2,\dots,k)$ (cluster assignments)
- minimize $f$ in terms of the $w_c$ (cluster centers)
#### Termination/convergence of the algorithm is guaranteed because:
- Each step does not increase the objective
	- will always be decrease $\rightarrow$ converge
- There are finite number of instance assignments to $k$ [[cluster(s)]] ($k^n$)
	- it cannot be larger than $k^n$
## Shape of [[k-Means]] [[cluster(s)]]
![[Pasted image 20240604145821.png]]
- [[k-Means]] partitions the input space into convex regions, with linear cluster boundaries
	- convex: if any line between 2 points in the region stays in the region![[Pasted image 20240604145740.png]]
- ##### Potential issues: True [[cluster(s)]] may not be convex
	- [[k-Means]] will fail if not convex
## Non-convex data sets
- being separated by just singular lines![[Pasted image 20240604145900.png]]
## Other issues of [[k-Means]]
![[Pasted image 20240604150003.png]]