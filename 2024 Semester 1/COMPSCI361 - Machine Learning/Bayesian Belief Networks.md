- where every node in the graph will be 1 variable (no more target/input variables)
- a simple, graphical notation for [[conditionally independent]] assertions and hence for compact specification of full joint distributions
## Syntax
- a set of nodes, one per random variable $X_i$
- a set of directed edges between the nodes, each edge represents the direction of influence among random variables
- a directed, acyclic graph (no cycles) - No loops
- A [[conditional probability]] distribution for each node given its parent nodes:
	- P