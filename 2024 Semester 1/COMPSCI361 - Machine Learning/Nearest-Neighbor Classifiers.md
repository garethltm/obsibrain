## Basic Idea
- find [[training data]] that are closest to this new point to support its prediction
- [[k-nearest neighbour (KNN)]]: Use $k$ "closest" training points ([[nearest neighbors]]) for performing the new point's [[classification]].
![[Pasted image 20240605094631.png]]
## Requires 3 things
1. The set of stored training instances (already labelled by humans)
2. Distance metric to compute distance between instances
3. The value of $k$, the number of [[nearest neighbors]] to retrieve
## To classify an unknown instance
- compute distance to other training instances
- Identify $k$ nearest neighbors
- Use class labels of the nearest neighbors to determine the class label of the unknown instance
	- #compsci361example by taking majority vote