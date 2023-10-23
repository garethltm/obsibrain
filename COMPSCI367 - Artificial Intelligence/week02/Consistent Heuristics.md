A **heuristic is consistent** if for every node n, every [[successor(s)]] of n’ of n generated for any [[action(s)]] a,
$$ h(n) ≤ c(n,a,n’) + h(n’) $$

If **h is consistent**, we have
$$ f(n’) 
= g(n’) + h(n’) = g(n) + c(n,a,n') + h(n') ≥ g(n) + h(n) ≥ f(n)

$$

- [[heuristic(s)]] “edge” cost ≤ actual cost for each edge

$$ |h(A) - h(C)|≤c(A,C) $$
OR
$$ h(C) - c(A,C) ≤ h(A) ≤ c(A,C) + h(C) $$

### Consequences of consistency
- The f value along a path never decreases:
    $$ h(A) ≤ c(A,C) + h(C) $$becomes
    $$ g(A) + h(A) ≤ g(A) + c(A,C) + h(C) $$
- [[A-Star Search]] is [[optimal]] (no-reopenings)