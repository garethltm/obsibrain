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

