- adaptation of [[Iterative Best Improvement (IBI)]] by maintaining ==M assignments==
	- where M ≥ 1 is a parameter
- fixed size 
	- therefore, memory is not needed
### Drawbacks
- tendency to focus on a limited set of solutions & potentially could get stuck on local optima, which can hinder its ability to explore the entire search space & find globally optimal solutions
## Steps
1. Initialise size-M [[population]] randomly $x1,...,xM$
2. At every step, examine all [[successor(s)]] of the current [[population]] $x1,...,xM$, pick the top M [[successor(s)]] that have the lowest cost (which are going to be the next [[population]])
3. Replace $x1,...,xM$ with these M [[successor(s)]]

![[Pasted image 20231022152110.png]]