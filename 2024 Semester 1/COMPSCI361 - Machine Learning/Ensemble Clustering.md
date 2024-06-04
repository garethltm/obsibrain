We can consider [[Ensemble(s)]] methods for [[Clustering]]: "consensus" [[Clustering]]
- Good/Important idea
	- [[Bootstrapping]] is widely-used
	- Do [[cluster(s)]] change if the data was slightly different?
- But we need to be careful about how we combine models
- #compsci361example run [[k-Means]] 20 times & then [[cluster(s)]] using the mode of the assigned [[cluster(s)]] labels $$
\{y_i^m | 1 \leq m \leq 20\}
$$
