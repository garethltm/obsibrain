uses proximity to make [[classification]] or predictions about the grouping of an individual data point.
## Algorithm
- all instances correspond to points in the $D$-dim space
- The [[nearest neighbor(s)]] are defined based on [[Euclidean distance]]:
	$$d_E(x, y) = \sqrt{\sum_{i=1}^{D}(x_i - y_i)^2}$$

- Target function could be [[Discrete-valued (Classification)]] or [[Real-valued (Regression)]]
## Hyperparameters
1. $Number\ of\ Neighbors\ (k)$: This is the $k$ value in the [[k-nearest neighbour (kNN)]] algorithm
2. $Distance\ Metric$: Distance metric to be used to compute distance between samples
	- [[Euclidean distance]]
