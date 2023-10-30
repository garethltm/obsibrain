- can be applied to reduce search cost
- a function that ==**estimates**== how close a [[state(s)]] is to a [[goal(s) - goal state(s)]]
- a [[solution(s)]] to relaxed problems, where some of the [[constraint(s)]] of the original problem have been removed

### Additional 
- Heuristics are “rules of thumb”
- Heuristics are criteria, methods or principles for deciding which among several alternative courses of [[action(s)]] promises to be the most effective in order to achieve some [[goal(s) - goal state(s)]]
- Can make use of [[heuristic(s)]] in deciding which is the most “promising” [[path(s)]] to take during search
- In search, ==[[heuristic(s)]] should be an underestimate of actual cost== to get from current node to any goal - an [[Admissible heuristic]]
- ==Denoted `h(n); h(n) = 0` when ever n is a [[goal(s) - goal state(s)]] node==

If Problem $p2$ is a relaxed version of $p1$ then
$$ h2*(n) ≤ h1*(n) $$
for every s, so $h2$*(n) is admissible for p1

![[Pasted image 20231023143837.png]]
With [[A-Star Search]]: a trade-off between quality of estimate and work per node
- As **[[heuristic(s)]] get closer to the true cost**, you will expand fewer nodes but usually do more work per node to compute the [[heuristic(s)]] itself
## Main idea
- in an ideal scenario where there are no limitation, what is the best possible [[solution(s)]]
##### What does $h1$ BETTER than $h2$ means (How do we know which [[heuristic(s)]] is better)
- What we’d like $h1$ better than $h2$ for problem P to mean is that [[A-Star Search]] solving P using takes less [[Time Complexity]] & [[Space Complexity]] than [[A-Star Search]] using [[heuristic(s)]]
- However. that is hard to predict in general
- So, instead we look at node expansions as a proxy for [[Time Complexity]] & [[Space Complexity]]
- If A* expands fewer nodes using $h1$ than using we say it is “better”
- Happily, we can characterise when this is likely to happen, namely when $h1$’s values are not lower than $h2$’s values
### Summary
- [[Admissible heuristic]]
- Comparing [[heuristic(s)]]
> Good [[heuristic(s)]] can help [[A-Star Search]] algorithm to find the [[solution(s)]] faster