![[Pasted image 20231022021423.png]]
- First in First Out
- [[Frontier]] = [[Queue]]
	- Selecting the earliest element to add to the [[Frontier]]
> If the list of [[path(s)]] on the [[Frontier]] is $(p1,p2,...,pr)$ :
	- $p1$ is selected. Its neighbours are added to the end of the [[Queue]], after $pr$
	- $p2$ is selected next
- All nodes are expanded at a given depth in the tree before any nodes at the next level are expanded
- Can be implemented by using a [[Queue]] to store [[Frontier]] nodes
    - put newly generated successors at end of [[Queue]]
- Stop when node with [[Goal(s) - Goal State(s)]] is generated
- Very systematic
- Find the shallowest [[Goal(s) - Goal State(s)]] first
### Complexity
- Does [[Breadth-First Search (BFS)]] guarantee to find the [[path(s)]] with fewest [[arc]]?
    - doesn’t mean we have an optimal solution where we can find a [[path(s)]] with fewest [[arc]]
- What happens on infinite graphs or on graphs with cycles if there is a solution?
    - graph with loops on it can be infinitely generated
- What is the [[Time Complexity]] as a function of the length of the [[path(s)]] selected?
    - limited in time running the algorithm
- What is the [[Space Complexity]] as a function of the length of the [[path(s)]] selected?
    - we need to allocate certain space for the [[Frontier]]
- How does the [[Goal(s) - Goal State(s)]] affect the search?

## Properties
1. [[Complete]]
	- it terminates with a [[solution(s)]] when one exists
2.  [[Time Complexity]]
	-  $+ b^2+b^3+…+b^d = O(b^d)$
3. [[Space Complexity]]
	- $O(b^d)$ - as it keeps every node in memory, where it generates all the nodes up to level d
4. [[Optimal]]
	- Yes - only if all the [[action(s)]] have the same cost

## Summary
- Space is a big problem - it grows exponentially with depth
- Good for fewest [[arc]]
- We will be searching till the reaching depth of our [[solution(s)]]
![[Pasted image 20231022023607.png]]