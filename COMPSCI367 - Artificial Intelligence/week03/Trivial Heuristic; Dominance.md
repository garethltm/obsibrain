![[Pasted image 20231023152108.png]]
Dominance: if $ha(n) ≥ hc(n)$ for all n (both [[Admissible heuristic]]) then $h2$ dominates $h1$ and is better for search.
So the aim is to make the [[heuristic(s)]] h() as large as possible, but without exceeding h*():
$ha ≥ hc$ if $∀n: ha(n) ≥ hc(n)$

Heuristics form a semi-lattice:

- Max of admissible heuristics is admissible
    
    $h(n) = max(ha(n) ≥ hb(n))$
    

Trivial heuristics

- Bottom of lattice is the zero heuristic (what does this give us?)
- Top of lattice is the exact heuristic