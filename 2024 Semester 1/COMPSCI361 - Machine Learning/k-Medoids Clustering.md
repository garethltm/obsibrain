A disadvantage of [[k-Means]] in some applications: the cluster centers might not be valid data points
#compsci361example consider document described by [[bag-of-words]] features like:
	[0,0,1,1,0], that is words 3 and 4 appear in the document
- A [[cluster(s)]] center from [[k-Means]] might look like [0.1 0.3 0.8 0.2 0.3] (synthetic solution)
- What does it mean to have 0.3 of word 2 in a document? - it doesn't compute
## Alternative to [[k-Means]] is [[k-Medoids Clustering]]
- Same algorithm as [[k-Means]], except the [[cluster(s)]] centres must be data points in D.
	- take one sample in your [[cluster(s)]] such that, it is the one that is closest to all others in terms of distance measured
- Update the cluster center by finding [[instance(s)]] in the [[cluster(s)]] minimizing squared L2-norm distance to all points in the [[cluster(s)]]
## Initialization
- [[k-Means]] is fast but sensitive to **Initialization**
- Classic approach to initialization: random restarts
	- run to convergence using different random initializations
	- Choose the one that minimizes average squared distances of data to the [[cluster(s)]] centers
		- choose the best one out of those several runs
- Newer approach: [[k-Means++]] (smartly chooses the centers)
