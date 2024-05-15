- [[Cluster]]
	- Similar (or related) to one another within the same group (same labels)
	- Dissimilar (or unrelated) to objects in other groups
## Motivation
#compsci361example Classifying Cancer Types
- We collected gene expression data for 8 cancer patients, can you find the types of cancer in the data?![[Pasted image 20240515163716.png]]
## General idea
- 2 data points that are similar are enclosed in a space - everything close is 1 cluster
![[Pasted image 20240413224824.png]]
![[Pasted image 20240515164136.png]]
![[Pasted image 20240515164111.png]]
- Input: set of [[instance(s)]] described by $d$ features
- Output: an assignment of [[instance(s)]] to 'groups' (no target class)
- Unlike [[classification]], we are not given the 'groups'
	- #### Task: Algorithm must discover groups
- #compsci361example groups we might discover in e-mail spam:
	- 'Lucky winner' group
	- 'Weight loss' group
	- 'I need your help' group
	- 'Mail-order bride' group

#compsci361questions 
## What [[Clustering]] does
- Detect and remove outliers
## Potential Problem
1. Information loss
2. There might be some outliers beyond the domain