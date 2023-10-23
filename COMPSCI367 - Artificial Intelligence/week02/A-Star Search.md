![[Pasted image 20231023150701.png]]
- combination of both [[Uniform-Cost Search (UCS) (Lowest-Cost-First Search)]] & [[Greedy (Best-First) Search]]

**[[Uniform-Cost Search (UCS) (Lowest-Cost-First Search)]]** 
- orders by **path cost** or backward cost: **g(n)**
**[[Greedy (Best-First) Search]]** 
- orders by **goal proximity** or forward cost: **h(n)**
*A-Star Search orders by the sum:* f(n) = **g(n)** + **h(n)**

## Main Idea
- Use both cost of path generated & estimate to goal to order nodes on the frontier
- **g(n) = cost of path from start to n**; **h(n) = estimate from n to goal**
- Order priority queue using function **f(n)** = **g(n)** + **h(n)**
- **f(n)** is the **estimated cost** of the **cheapest solution** extending this path