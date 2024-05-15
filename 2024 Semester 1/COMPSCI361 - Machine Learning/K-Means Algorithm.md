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
		- such that the some [[instance(s)]] are closer to ot