We can consider [[Ensemble(s)]] methods for [[Clustering]]: "consensus" [[Clustering]]
- Good/Important idea
	- [[Bootstrapping]] is widely-used
	- Do [[cluster(s)]] change if the data was slightly different?
- But we need to be careful about how we combine models
- #compsci361example run [[k-Means]] 20 times & then [[cluster(s)]] using the mode of the assigned [[cluster(s)]] labels $\{y_i^m | 1 \leq m \leq 20\}$ for the $i$-th [[instance(s)]]
- Normally, averaging across models doing different things is good
- But this is a bad [[Ensemble(s)]] method: worse than [[k-Means]] on its own
## Idea for [[Ensemble Clustering]]
1. Run [[k-Means]] $m$ times with different initialization to produce $m$ [[Clustering]] outputs
2. For each pair of [[instance(s)]] $x_i$ & $x_j$, define
	- $m_{ij}$, the number times both [[instance(s)]] are in the same [[cluster(s)]]
	- $p_{ij}=\frac {m_{ij}}{m}$, the probability the [[instance(s)]] are clustered together
3. Put $x_i$ and $x_j$ in the same [[cluster(s)]] if $p_{ij}>0.5$
	- If both are already assigned to [[cluster(s)]], merge both [[cluster(s)]]
	- If none are assigned, form a new [[cluster(s)]]
	- If only one is assigned, assign the other one into the same [[cluster(s)]]
Note: some points are not assigned to any [[cluster(s)]]
You can implement this with a [[DBSCAN]] code (just "distance" changes)
