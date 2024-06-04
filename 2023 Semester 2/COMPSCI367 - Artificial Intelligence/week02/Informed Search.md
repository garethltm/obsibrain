## Summary
- All of them uses [[heuristic(s)]].
	- [[heuristic(s)]] can be applied to reduce search cost
	- In order to find [[heuristic(s)]], you need to solve a relaxed problem and think of what kind on constraints you can ignore and decide on what actions that brings you closer to your [[Goal(s) - Goal State(s)]]
	- Working on [[closed list]]/[[frontier (open list, fringe)]] can affect the [[Time Complexity]] & [[Space Complexity]] used of the algorithm
- [[Greedy (Best-First) Search]] tries to minimise the cost from current node n to the goal
- [[A-Star Search]] combines the advantages of Uniform-Cost Search & Greedy Search
	- [[A-Star Search]] is [[Complete]], [[Optimal]] and optimally efficient among all optimal search algorithms
	- [[Space Complexity]] is still a concern for [[A-Star Search]]: [[Iterative Deepening A-Star Search (IDA)]] is a low-memory variant
- [[Informed Search]] makes use to problem-specific knowledge to guide progress of search
	- This can lead to a significant improvement in performance
	- Much research has gone into [[Admissible heuristic]]
	    - Even on the automatic generation of [[Admissible heuristic]]

- [[Informed Search]] strategy
    - one that uses problem-specific knowledge beyond the definition of the problem itself
    - can find solutions more efficiently than uninformed strategy
- Informed search algorithms, can do quite well given some guidance on where to look for solutions
- All implemented using a [[Priority Queue]] to store [[frontier (open list, fringe)]] nodes

# Types of Informed Search
- [[Greedy (Best-First) Search]]
- [[A-Star Search]]
- [[Iterative Deepening A-Star Search (IDA)]]