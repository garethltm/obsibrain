Chi-merge: $\chi  ^2$-based [[Discretization]]
- [[Supervised Learning]]: use class information
- Bottom-up merge: find the best neighbouring intervals (those having similar distributions of classes #compsci361example low $\chi ^2$ values) to merge
- Merge performed recursively, until a predefined stopping condition

#compsci361example Given 2 nominal variables C and B with values $c\tiny {1}\normalsize,...,c\tiny {k}$ & $b\tiny {1}\normalsize,...,b\tiny {r}$ the correlation can be calculated using the $\chi ^2$ test:
$$\chi ^2 = \displaystyle\sum_{i=1}^k \displaystyle\sum_{j=1}^r \frac {(o\tiny {ij}\normalsize -e\tiny{ij}\normalsize)}{}$$
