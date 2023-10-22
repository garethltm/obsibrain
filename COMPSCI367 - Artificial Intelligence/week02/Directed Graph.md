- Consists of 
	- a set of N of nodes
	- a set of A of [[Arc]] where an [[Arc]] is an ordered pair of nodes
		- The [[Arc]] <n1, n2> is an outgoing [[Arc]] from n1 & an incoming [[Arc]] to n2
	- a [[Path]]
	- a [[Goal]] is a boolean function on nodes. If goal(n) is true, then we can conclude that node n satisfies the [[Goal]] & n is a [[Goal]] node
To encode problems as graphs:
1. One node is identified as Start Node
2. A [[Solution]] is a [[Path]] from Start Node to a node that satisfies that [[Goal]]





