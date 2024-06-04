## Complexity
Computational complexity of basic implementation is $O(n^3)$
- it is extremely expensive $\rightarrow$ because they are mostly pairwise comparisons
- One step costs $O(n^2d)$: (standard) distance calculation, $O(d)$, between up to $n^2$ points.
- At most $O(n)$ steps: Starting with $n$ singleton [[cluster(s)]] & merging 2 [[cluster(s)]] in each step, after $O(n)$ steps only 1 [[cluster(s)]] will be left
This can be reduced to $O(n^2d\times log(n)$ with a [[Priority Queue]](optimisation): store distances in a sorted order, only update the distances that change
## Pseudocode
![[Pasted image 20240604164930.png]]