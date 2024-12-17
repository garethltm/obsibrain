- where every node in the graph will be 1 variable (no more target/input variables)
- a simple, graphical notation for [[conditionally independent]] assertions and hence for compact specification of full joint distributions
## Syntax
- a set of nodes, one per random variable $X_i$
- a set of directed edges between the nodes, each edge represents the direction of influence among random variables
- a directed, acyclic graph (no cycles) - No loops
- A [[conditional probability]] distribution for each node given its parent nodes:
	- $P(X_i|Parents(X_i))$
- Conditional distribution represented as a [[Conditional Probability Table (CPT)]] giving the distribution of $X_i$ for each combination of parent values
## Variable Relationships
- a graphical model of relationships
1. Encodes dependencies among the variables (can be causal dependencies)
	- $X$ is a parent of $Y$, if there is a directed edge from $X$ to $Y$
	- $X$ is an ancestor of $Y$ 
	- $Y$ is a descendant of $X$ 
		- if there is a directed path in the graph from $X$ to $Y$
		- #compsci361example ![[Pasted image 20240515000058.png]]
		- $X_1, X_2$ are parents of $X_3$
		- $X_2$ is the parent of $X_4$
		- $X_2$ has no ancestors/parents, but $X_2$ is ancestor of $X_3,X_4$ and $X_5$
		- [[University of Auckland/2024 Semester 1/COMPSCI361 - Machine Learning/Local Markov property|Local Markov property]]
2. Gives a specification of the joint probability distribution
	- If we label the nodes such that $X_i$ is an ancestor of $X_j$ only if $i < j$ , the joint probability can be factorized chain rule of [[University of Auckland/2024 Semester 1/COMPSCI361 - Machine Learning/Probability|Probability]] and [[University of Auckland/2024 Semester 1/COMPSCI361 - Machine Learning/Local Markov property|Local Markov property]] as:
	- ### Chain Rule
		- The chain rule in probability can be expressed as:
		- $P(X_1, \ldots , X_n) = P(X_1) P(X_2|X_1) \ldots P(X_n|X_{n-1})$
		- You only need to know the parents of the variable.
		- You only care about the cases you have direct links.
	- ### Non-descendants of ($X_i$)
		- The probability of non-descendants of ($X_i$) can be written as:
			- $\prod_{i=1}^n P(X_i | X_1, X_2, \ldots , X_{i-1})$
	- ### Parents of ($X_i$)
		- The probability considering only the parents of ($X_i$) is given by:
			- $\prod_{i=1}^n P(X_i|\text{Parents}(X_i))$
	- #compsci361example ![[Pasted image 20240515000058.png]]$P(X_1, X_2, X_3, X_4, X_5) = P(X_1)P(X_2)P(X_3|X_1,X_2)P(X_4|X_2)P(X_5|X_4)$

#compsci361example ![[Pasted image 20240515161311.png]]
### Joint probability
![[Pasted image 20240515161341.png]]
#compsci361example ![[Pasted image 20240515161404.png]]



