- adaptation of [[Iterative best improvement]] by maintaining M assignments
	- where M ≥ 1 is a parameter

## Steps
1. Initialise size-M [[population]] randomly $x1,...,xM$
2. At every step, examine all [[successor(s)]] of the current [[population]] $x1,...,xM$, pick the top M [[successor(s)]] that have the lowest cost (which are going to be the next [[population]])
3. Replace $x1,...,xM$ with these M [[successor(s)]]

![[Pasted image 20231022152110.png]]