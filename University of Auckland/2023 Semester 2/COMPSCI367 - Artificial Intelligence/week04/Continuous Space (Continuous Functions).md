![[Pasted image 20231023173820.png]]

## Optimisation of Continuous Functions
- [[Discretisation]]
	- we can then apply a [[Manhattan distance]]
		- which we then can use [[Hill-Climbing]] (Discrete [[Local Search]])
- [[Gradient descent]] - we would be computing the [[gradient]] = iteratively updating the positions
	- make a move in the direction of the [[gradient]]

## Handling a Continuous State/Action Space
1. [[Discretisation]]
2. Choose random perturbations to the [[State(s)]]
	- [[First Choice Hill-Climbing]]: keep trying until something improves the [[State(s)]]
	- [[Simulated Annealing]]
3. Compute [[gradient]] of f(x) analytically