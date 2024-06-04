This doesn't work because of the [[Label Switching Problem]]
- The cluster labels $\hat{y_i}$ are meaningless
- We could get same [[Clustering]] with permuted labels ("exchangeable" labels)![[Pasted image 20240604161124.png]]
- All $\hat{y_i}$ become equally likely as number of initializations increases
- [[Ensemble(s)]] can't depend on label "meaning"
	- Don't ask: Is point $x_i$ in red square cluster?, which is meaningless
	- Ask: Is point $x_i$ in the same cluster as $x_j$?, which is meaningful