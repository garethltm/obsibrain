[[k-nearest neighbor (kNN)]] returns the mean values among the $k$ training examples nearest to $x'$
#compsci361example ![[Pasted image 20240605100429.png]]
## Prediction
[[k-nearest neighbor (kNN)]] for real-valued prediction for a given unknown input $\rightarrow$ [[Regression]] Problem
- Returns the mean values of its [[k-nearest neighbor (kNN)]]
[[Weighted kNN]] (a variant of normal [[k-nearest neighbor (kNN)]]): Distance-weighted [[nearest neighbor(s)]] algorithm
1. Weight the contribution of each of the $k$ neighbors according to the query $x'$
2. Give greater weight to closer neighbors:
	- $w=\frac {1}{d(x',x_i)}$
	- lesser weight to further neighbors
### Issue
- [[Noisy data]]: distance between neighbors could be dominated by irrelevant attributes
### Fix
- Elimination of the least relevant attributes
	- #compsci361example by applying [[Principal Components Analysis (PCA)]] on data before using [[k-nearest neighbor (kNN)]]