![[Pasted image 20231023152108.png]]
Dominance: if $ha(n) ≥ hc(n)$ for all n (both [[Admissible heuristic]]) then $h2$ dominates $h1$ and is better for search.
- So the aim is to make the [[heuristic(s)]] h() as large as possible, but without exceeding h*(): 
	- $ha ≥ hc$ if $∀n: ha(n) ≥ hc(n)$ - we prefer ha because it is dominating hc

[[heuristic(s)]] form a semi-lattice:
- Max of [[Admissible heuristic]] is admissible
	-  $h(n) = max(ha(n) ≥ hb(n))$ - in relation to 2 different [[heuristic(s)]]

Trivial [[heuristic(s)]]
- Bottom of lattice is the zero [[heuristic(s)]] (what does this give us?)
	- Gives:
		- [[Uniform-Cost Search (UCS) (Lowest-Cost-First Search)]]
		- if [[heuristic(s)]] goves
- Top of lattice is the exact [[heuristic(s)]]