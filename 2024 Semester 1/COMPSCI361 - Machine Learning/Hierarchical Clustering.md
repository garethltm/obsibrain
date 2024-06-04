[[Hierarchical Clustering]] produces a tree of [[cluster(s)]] or [[dendrogram]]
- Given a data set $D$, a [[dendrogram]] is a binary tree with elements of $D$ at its leaves
- An internal node of the tree represents the subset of elements in the leaves of the subtree rooted at that node
- The level (height) of a node is the distance between the 2 [[cluster(s)]] represented by the children of the node
- Leaves have level 0
	- all the levels will be at height = 0
- Each internal node in the tree splits the data into 2 or more [[cluster(s)]]
Heuristic that needs similarity/distance matrix to guide the [[Clustering]] process.
![[Pasted image 20240604164636.png]]
- refer to [[dendrogram]]
1. agglomerative
2. divisive
## Motivation
- Consider [[Density-Based Clustering]] on this data:![[Pasted image 20240604162912.png]]
- Increase $\epsilon$ & run it again:![[Pasted image 20240604162947.png]]
- More complicated case:![[Pasted image 20240604163021.png]]
## Note
When you are calculating [[cluster(s)]], there is no reason to think about hierarchy $\rightarrow$ main point is to find groups
- The hierarchical structure is returned whether there exists 1 in the data or not
	- How would the [[dendrogram]] look if there is no structure in the data?
- A [[dendrogram]] is the description of the result of the algorithm, not a graphical