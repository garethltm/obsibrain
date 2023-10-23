![[Pasted image 20231023150701.png]]
- combination of both [[Uniform-Cost Search (UCS) (Lowest-Cost-First Search)]] & [[Greedy (Best-First) Search]]

**[[Uniform-Cost Search (UCS) (Lowest-Cost-First Search)]]** 
- orders by **path cost** or backward cost: **g(n)**
**[[Greedy (Best-First) Search]]** 
- orders by **goal proximity** or forward cost: **h(n)**
*A-Star Search orders by the sum:* f(n) = **g(n)** + **h(n)**

[[Uniform-Cost Search (UCS) (Lowest-Cost-First Search)]] minimizes **g(n)**
- [[optimal]] & [[complete]] but not efficient
[[Greedy (Best-First) Search]] minimizes **h(n)**
- efficient but not [[optimal]] or [[complete]]

## Main Idea
- Use both cost of path generated & estimate to goal to order nodes on the [[frontier]]
- **f(n)** is the **estimated cost** of the **cheapest solution** extending this [[path(s)]] (through node n)
- **g(n) = cost of path from [[Initial State (Start State)]] to n**; 
- **h(n) = estimate from n to [[Goal(s) - Goal State(s)]]**
- Order [[priority queue]] using function **f(n)** = **g(n)** + **h(n)**

### Heuristic Function

