There are $2^d -1$ possible attribute combinations of $d$ attributes
- exhaustive search is not feasible #compsci361example d = 300 features, $2.04 \times 10^{90}$ combinations 
### Typical heuristic [[Attribute (Feature) selection]] methods:
1. Best single attribute under the attribute independence assumption
2. Best Step-wise [[Attribute (Feature) selection]]: (Adding features 1 by 1)
	- The best single-attribute is picked first
	- Then next best attribute condition to the first
3. Step-wise Attribute elimination: (Remove features 1 by 1)
	 - Repeatedly eliminate the worst attribute
4. Best combined attribute selection & elimination
5. Optimal branch & bound:
	- Use attribute & [[Backtracking Search]]
