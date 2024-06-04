A disadvantage of [[k-Means Algorithm]] in some applications: the cluster centers might not be valid data points
#compsci361example consider document described by [[bag-of-words]] features like:
	[0,0,1,1,0], that is words 3 and 4 appear in the document
- A [[cluster(s)]] center from [[k-Means Algorithm]] might look like [0.1 0.3 0.8 0.2 0.3] (synthetic solution)
- What does it mean to have 0.3 of word 2 in a document? - it doesn't compute
## Alternative to [[k-Means Algorithm]] 