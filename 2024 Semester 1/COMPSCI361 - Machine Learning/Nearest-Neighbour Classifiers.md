## Basic Idea
- find [[training data]] that are closest to this new point to support its prediction
- [[k-nearest neighbour (KNN)]]: Use $k$ "closest" training points (nearest neighbours) for performing the new point's [[classification]].
![[Pasted image 20240605094631.png]]
## Requires 3 things
1. The set of stored training instances (already labelled by humans)
2. Distance metric to compute distance between instances
3. The value of $k$, the number of nearest neighbours to retrieve
## To classify an unknown instance
- compute distance to other training instances
- Identify $k$ nearest neighbours
- Use class labels of the nearest neighbours to determine the class label of the unknown ins