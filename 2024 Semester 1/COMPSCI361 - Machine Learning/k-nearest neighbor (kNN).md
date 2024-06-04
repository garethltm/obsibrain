uses proximity to make [[classification]] or predictions about the grouping of an individual data point.
## Algorithm
- all instances correspond to points in the $D$-dim space
- The [[nearest neighbor(s)]] are defined based on [[Euclidean distance]]:
- Target function could be [[Discrete-valued (Classification)]] or [[Real-valued (Regression)]]
## Hyperparameters
1. $Number\ of\ Neighbors\ (k)$: This is the $k$ value in the [[k-nearest neighbor (kNN)]] algorithm
2. $Distance\ Metric$: Distance metric to be used to compute distance between samples
	![[Pasted image 20240605101901.png]]
	- [[Euclidean distance]]
	- [[Manhattan distance]]
## Choice of $k$
![[Pasted image 20240605102004.png]]
1. If $k$ is too small, sensitive to [[Noise]] points
2. If $k$ is too large, neighborhood may include points from other classes
## What's the impact of $k$?
- [[Euclidean distance]]![[Pasted image 20240605102032.png]]

- [[Manhattan distance]]![[Pasted image 20240605102122.png]]
## Decision boundaries of [[k-nearest neighbor (kNN)]]
- [[k-nearest neighbor (kNN)]] produces decision boundaries of arbitrary shape
- Provide more flexibility compared to [[rule-based classifiers]]
- High variety because decision boundaries depends on training samples in the local neighborhood
- [[Vonoroi diagram (1-NN)]]
## Issues
1. Scaling Issue
	#compsci361example 
	- height of a person may vary from 1.5m to 1.8m
	- weight of a person may vary from 90lb to 300lb
	- income of a person may vary from $10k to $1M
	**Solution**: Attributes may have to be scaled ([[Normalization]]) to prevent distance measures from being dominated by one of the attributes:
	1. Irrelevant & Redundant Attributes Issue
		- Irrelev