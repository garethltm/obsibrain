A **heuristic is consistent** if for every node n, every successor of n’ of n generated for any action a,
$$ h(n) ≤ c(n,a,n’) + h(n’) $$

If **h is consistent**, we have
$$ f(n’) = g(n’) + h(n’) = g(n) + c(n,a,n') + h(n') ≥ g(n) + h(n) ≥ f(n)

$$

