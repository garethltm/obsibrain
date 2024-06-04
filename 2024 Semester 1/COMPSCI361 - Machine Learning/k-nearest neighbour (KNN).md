uses proximity to make [[classification]] or predictions about the grouping of an individual data point.
## Algorithm
- all instances correspond to points in the $D$-dim space
- The [[nearest neighbor(s)]] are defined based on Euclidean distance:
- Sure, here's the equation converted to Markdown syntax using LaTeX: $$d_E(x, y) = \sqrt{\sum_{i=1}^{D}(x_i - y_i)^2}$$
	- $x$ = old training point
	- $y$ = new training point
- Target function could be [[Discrete-valued (Classification)]] or [[Real-valued (Regression)]]
## Hyperparameters
1. $Number\ of\ Neighbors\ (k)$: This is the $k$ value in the [[knn]]
