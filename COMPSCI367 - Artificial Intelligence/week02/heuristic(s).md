- a [[solution(s)]] to relaxed problems, where some of the [[constraint(s)]] of the original problem have been removed
- Heuristics are “rules of thumb”
- Heuristics are criteria, methods or principles for deciding which among several alternative courses of [[action(s)]] promises to be the most effective in order to achieve some [[Goal(s) - Goal State(s)]]
- Can make use of heuristics in deciding which is the most “promising” [[path(s)]] to take during search
- In search, heuristic should be an underestimate of actual cost to get from current node to any goal - an [[Admissible heuristic]]
- Denoted `h(n); h(n) = 0` when ever n is a [[Goal(s) - Goal State(s)]] node

If Problem $p2$ is a relaxed version of $p1$ then
$$ h2*(n) ≤ h1*(n) $$
for every s, so $h2$*(n) is admissible for p1

![[Pasted image 20231023143837.png]]

## Main idea
- in an ideal scenario where there are no limitation, what is the best possible [[solution(s)]]

### Summary
- [[Admissible heuristic]]
- Comparing [[heuristic(s)]]
> Good [[heuristic(s)]] can help [[A-Star Search]] algorithm to find the [[solution(s)]] faster